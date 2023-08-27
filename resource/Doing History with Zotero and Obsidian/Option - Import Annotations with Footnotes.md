
![copy footnote.png](res/copy%20footnote.png)

_Note: Because this setup requires fiddling with Zotero, it is not in the starter [Obsidian history vault](https://github.com/erazlogo/obsidian-history-vault). When Zotero Integration adds an option to import footnote citation with annotations, this feature will be included in the vault._

If you write in Scrivener or Ulysses and use footnote styles you may prefer to import annotations with a footnote citation instead of a bibliographic reference. This would allow you to copy the footnote citation quickly into another program while writing.

Eventually, this will be possible via Zotero Integration preferences, but for now you can use a workaround: add a CSL ([citation style language](https://citationstyles.org/)) file to use for footnoting in Zotero styles folder.

### Import annotations with a footnote

First, duplicate the CSL file you usually use for references in your `zotero/styles/` folder (in my case, `zotero/styles/chicago-fullnote-bibliography.csl`)

![duplicate csl file.png](res/duplicate%20csl%20file.png)  
Rename the new file to include "citation" in the title (in my case, "chicago-fullnote-citation.csl").

Open the new file in any text editor, for example TextEdit.

![open csl file in text editor.png](res/open%20csl%20file%20in%20text%20editor.png)  
At the top of the file, change the name the style to the new name on three lines, for title, id, and link.

![change csl id.png](res/change%20csl%20id.png)  
Scroll all the way down, and replace two instances of "bibliography" with "citation," and vice versa.

![edit csl file.gif](res/edit%20csl%20file.gif)

In Zotero, add the new style to the QuickCopy preferences:

![add style to zotero preferences.png](res/add%20style%20to%20zotero%20preferences.png)  
In Obsidian, add the new style to the Import settings. Make sure that to hit `Enter` after you paste the name of the style and doublecheck that it stays in the field after you close the dialogue.

![add name to import settings.png](res/add%20name%20to%20import%20settings.png)

### Add page number to footnote on import

Next, set up your template to add the page number for the quote to the footnote reference on import.

First, make sure that the annotation pages are correct in Zotero, and fix them if they are not:

![fix page numbers.png](res/fix%20page%20numbers.png)  
Replace your import template (in my case, it is located in `meta/zotero/research note.md`) with this new template:

```
---
type: "{{itemType}}"{% for type, creators in creators | groupby("creatorType") -%}{% if loop.first %}
{% endif %}{{type | replace("interviewee", "author") | replace("director", "author") | replace("presenter", "author") | replace("podcaster", "author") | replace("programmer", "author") | replace("cartographer", "author") | replace("inventor", "author") | replace("sponsor", "author")  | replace("performer", "author") | replace("artist", "author")}}: "{%- for creator in creators -%}{%- if creator.name %}{{creator.name}}{%- else %}{{creator.lastName}}, {{creator.firstName}}{%- endif %}{% if not loop.last %}; {% endif %}{% endfor %}"{% if not loop.last %}
{% endif %}{%- endfor %}{% if title %}
title: "{{title}}"{% endif %}{% if publicationTitle %}
publication: "{{publicationTitle}}"{% endif %}{% if date %}
date: {{date | format("YYYY-MM-DD")}}{% endif %}{% if archive %}
archive: "{{archive}}"{% endif %}{% if archiveLocation %}
archive-location: "{{archiveLocation}}"{% endif %}
citekey: {{citekey}}
---
{% if ((itemType == "journalArticle") or (itemType == "bookSection")) and pages.length %}{{ bibliography | truncate(bibliography.length - (pages.length + 1), true, " ") }}{% else %}{{ bibliography | truncate(bibliography.length - 1, true, ", ") }}{% endif %}{% for annotation in annotations %}{% if loop.first %}{{annotation.pageLabel}}{% endif %}{% endfor %}
[online]({{uri}}) [local]({{desktopURI}}) {%- for attachment in attachments | filterby("path", "endswith", ".pdf") %} [pdf](file://{{attachment.path | replace(" ", "%20")}})
{%- endfor -%}
 
{% if tags.length > 0 -%}{% for t in tags -%}{% if t.tag == "secondary" %}

#source/secondary{% elif t.tag == "primary" %}

#source/primary{% elif "-project" in t.tag %}
#project/{{t.tag | replace("-project", "")}}{% endif %}{%- endfor %}{%- endif %}

### Index

start-date:: {% if date %}{{date | format("YYYY-MM-DD")}}{% endif %}
end-date::
page-no:: {% for annotation in annotations %}{% if loop.first %}{{annotation.pageLabel}}{% endif %}{% endfor %}

### Connections

comment:: 

### Note
{%- for annotation in annotations %}
{% if annotation.imageRelativePath %}
![[{{annotation.imageRelativePath}}]] {% endif %}{% if annotation.annotatedText %}
{{annotation.annotatedText}} [(p. {{annotation.pageLabel}})](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.pageLabel}}&annotation={{annotation.id}}){%- endif %}{%- if annotation.comment%}
%%{{annotation.comment}}%%{%- endif %}{%- endfor %}
```

Now, when you import annotations from Zotero, the script will add the page number for the first highlight to the footnote citation and the `page-no field`:

![import annotations with pages.gif](res/import%20annotations%20with%20pages.gif)

### Set page number for extracted research note

Next, set up your script to set the correct page number when you extract an individual research note from your import. To do that, replace javascript in your `header.js` file (in my case, in `meta/javascript/header.js`) with this script (omit accents in the beginning and the end):

```
function header(tp) {
    content=tp.file.content;
    selection=tp.file.selection();
    getheader=content.substring(0, content.indexOf("### Note")+10);
    pageno=selection.substring(selection.indexOf("?page=")+6, selection.indexOf("&annotation"));
    oldpageno=getheader.substring(getheader.indexOf("page-no:: ")+10, getheader.indexOf("\n", getheader.indexOf("page-no:: ")+10));
    headerwithpageno=getheader.replace("page-no:: "+oldpageno+"\n", "page-no:: "+pageno+"\n").replace(oldpageno+"\n[online]", pageno+"\n[online]");
     return headerwithpageno;
}
module.exports = header;
```

Now when you extract an individual reference note the correct page number will be added to the footnote citation and the `page-no field`:

![extract annotation with pages.gif](res/extract%20annotation%20with%20pages.gif)

Et viola! You have a formatted footnote you can copy to your favorite writing app.