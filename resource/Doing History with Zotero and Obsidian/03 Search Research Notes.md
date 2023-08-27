
![reddit question research notes.png](res/reddit%20question%20research%20notes.png)

_Note: All Obsidian plugins, scripts, and settings described here are included in the starter [Obsidian history vault](https://github.com/erazlogo/obsidian-history-vault) available for download on Github._

One history graduate student on Reddit (abridged above - see [full discussion](https://www.reddit.com/r/ObsidianMD/comments/vne0k5/question_on_research_notes_in_obsidianfeel_like/)) recently pointed to a key difference between historical research and the popular way of taking notes in Obsidian: historians need to record a lot of exact quotes and factual notes from sources. Elsewhere I explain how to [[01 Notetaking for Historians|create research notes]] with full citation, page numbers, and exact text from the source. But entering hundreds of research notes is just a start. In order to get to your own writing faster, you need a quick and easy search interface for these notes.

The regular Obsidian search (the magnifying glass on the top left) works well in general, but it cannot search your research notes by source fields, note text, your own comments, and sort them by event date, for example. To do that, I created a library-catalog search interface for my research notes:

![search research notes.gif](res/search%20research%20notes.gif)

All you have to do is to enter search terms into one or more fields to start searching.

Keyword search finds a word or phrase in the entire note text + note title.  
For text fields, this is a case-insensitive phrase search.  
Enter dates as `YYYY-MM-DD`, `<YYYY-MM-DD` and `>YYYY-MM-DD`.  
Enter tags as `#tag1 #tag2`.  
Enter exact field title and `asc/desc` to sort by field.  
Leave sort fields blank to sort by `note-title, desc`.

Below, I explain how to get to this point.

### Set Up the Search Page and Script

Necessary plugins and settings in Obsidian:

- Live Preview: On
- Dataview plugin
- Your research notes should reside in a separate folder in your vault (`01 notes` in my case)

If you haven't already, install the Dataview plugin via Community Plugins in Settings. In Dataview preferences, turn on "Enable Javascript Queries":

![dataview enable javascript.png](res/dataview%20enable%20javascript.png)  
Then change date format for proper sorting:

![dataview set date format.png](res/dataview%20set%20date%20format.png)

Place search files in any folder in your vault outside of your literature notes folder (in my case `meta/dataview`)

Create a separate note outside of your notes folder (in my case, `meta/dataview/Search Research Notes.md`). This note has search fields and calls the main script from another file, `search-research-notes.js.

````

keyword:: 

author:: 
recipient:: 
title:: 
publication:: 
date:: 
archive:: 
archive-location:: 

note-created:: 
note-modified:: 
note-title:: 

start-date:: 
end-date:: 
comment:: 
tags::   

sortby:: start-date
sortorder:: asc

```dataviewjs
await dv.view("meta/dataview/search-research-notes", { });
```
````

In a separate folder (in my case, `meta/dataview/search-research-notes`) create a file `search-research-notes.js`. The main script needs to be in a separate file because it is too long to work with Live Preview.

```
const current = dv.current();
const cdate = new Date(dv.current().date).getTime();
const cdateop = !dv.current().date ? "" : (dv.current().date.toString().includes("<") ? "<" : (dv.current().date.toString().includes(">") ? ">" : "==="));
const cnotecreated = new Date(dv.current()["note-created"]).getTime();
const cnotecreatedop = !dv.current()["note-created"] ? "" : (dv.current()["note-created"].toString().includes("<") ? "<" : (dv.current()["note-created"].toString().includes(">") ? ">" : "==="));
const cnotemodified = new Date(dv.current()["note-modified"]).getTime();
const cnotemodifiedop = !dv.current()["note-modified"] ? "" : (dv.current()["note-modified"].toString().includes("<") ? "<" : (dv.current()["note-modified"].toString().includes(">") ? ">" : "==="));
const cstartdate = new Date(dv.current()["start-date"]).getTime();
const cstartdateop = !dv.current()["start-date"] ? "" : (dv.current()["start-date"].toString().includes("<") ? "<" : (dv.current()["start-date"].toString().includes(">") ? ">" : "==="));
const cenddate = new Date(dv.current()["end-date"]).getTime();
const cenddateop = !dv.current()["end-date"] ? "" : (dv.current()["end-date"].toString().includes("<") ? "<" : (dv.current()["end-date"].toString().includes(">") ? ">" : "==="));
const matchtags = (a, b) => {
    for (const v of new Set(a)) {
      if (
        !b.some(e => e === v) ||
        a.filter(e => e === v).length > b.filter(e => e === v).length
      )
        return false;
    }
    return true;
};

if (current.keyword || current.author || current.recipient || current.title || current.publication || current.date || current.archive || current["archive-location"] || current["note-title"] || current["start-date"] || current["end-date"] || current["note-created"] || current["note-modified"] || current.comment || current.tags) {

    function passes(page) {
        return (!current.author || (page.author && page.author.toString().toLowerCase().includes(current.author.toLowerCase())))
            && (!current.recipient || (page.recipient && page.recipient.toString().toLowerCase().includes(current.recipient.toLowerCase())))
            && (!current.title || (page.title && page.title.toString().toLowerCase().includes(current.title.toLowerCase())))
            && (!current.publication || (page.publication && page.publication.toString().toLowerCase().includes(current.publication.toLowerCase())))
            && (!current.date || (page.date && eval(new Date(page.date).getTime() + cdateop + cdate)))
            && (!current.archive || (page.archive && page.archive.toLowerCase().includes(current.archive.toLowerCase())))
            && (!current["archive-location"] || (page["archive-location"] && page["archive-location"].toLowerCase().includes(current["archive-location"].toLowerCase())))
            && (!current["note-title"] || (page.file.name && page.file.name.toLowerCase().includes(current["note-title"].toLowerCase())))
            && (!current.comment || (page.comment && page.comment.toLowerCase().includes(current.comment.toLowerCase())))
            && (!current["start-date"] || (page["start-date"] && eval(new Date(page["start-date"]).getTime() + cstartdateop + cstartdate)))
            && (!current["end-date"] || (page["end-date"] && eval(new Date(page["end-date"]).getTime() + cenddateop + cenddate)))
            && (!current["note-created"] || (page.file.cday && eval(new Date(page.file.cday).getTime() + cnotecreatedop + cnotecreated)))
            && (!current["note-modified"] || (page.file.mday && eval(new Date(page.file.mday).getTime() + cnotemodifiedop + cnotemodified)))
            && (!current.tags || matchtags(current.file.tags, page.file.tags))
            ;
    }

    function keyword(page) {
        return (!current.keyword || (page.content && page.content.toLowerCase().includes(current.keyword.toLowerCase()))
            || (page.notetitle && page.notetitle.toLowerCase().includes(current.keyword.toLowerCase())))
            ;
    }

    const pages = await Promise.all(
        dv.pages('"01 notes"')
        .where(passes)
        .sort(p => ({ "note-created": p.file.ctime, "note-modified": p.file.mtime, "note-title": p.file.name }[current.sortby] ?? p[current.sortby]), current.sortorder)        
        .map(page => new Promise(async (resolve, reject) => {
            const content = await dv.io.load(page.file.path);
            resolve({
                link: page.file.link,
                startdate: page["start-date"],
                enddate: page["end-date"],
                author: page.author,
                recipient: page.recipient,
                title: page.title,
                publication: page.publication,
                date: page.date,
                pageno: page["page-no"],
                archive: page.archive,
                archivelocation: page["archive-location"],
                notetitle: page.file.name,
                comment: page.comment,
                content
            });
        }))
    );

    dv.table(
        ["Note Title", "Start Date", "End Date", "Author", "Recipient", "Title", "Publication", "Date", "Pages", "Archive", "Loc. in Archive"],
            pages
            .filter(keyword)
            .map(p => [
                p.link,
                p.startdate,
                p.enddate,
                p.author,
                p.recipient,
                p.title,
                p.publication,
                p.date,
                p.pageno,
                p.archive,
                p.archivelocation
            ])
    );
} else {
    dv.paragraph("   Enter search terms into one or more fields to find research notes.");
}
```

This script searches all notes in your research notes folder ( `01 notes` in my case).

### Add Minimal Theme to Display Search Results

Because the results list for this search has many columns, you need to use full screen width to display it. By default, Obsidian narrows down all text in the pane to readable length. This is useful for reading notes but does not work for the search. There are several ways to modify this setting, including adding a css snippet or using a theme that has special width setting for tables. I use the Minimal theme because it has a simple preference that keeps table width to 100%.

Install the following:

- Minimal theme, from Settings -> Appearance -> Themes
- Minimal Theme Settings plugin, from Community Plugins
- Contextual Typography plugin, from Community Plugins (required plugin for this theme)

In Minimal Theme Settings, set "Table width" to "100% pane width", and "Trim Dataview columns" off. The second setting will allow search results to display long text in your columns.

![minimal theme settings.png](res/minimal%20theme%20settings.png)

### Set Up Workspaces

The search script provides links to display individual research notes on their own, but I like to work in a view that allows me to see the graph of linked notes. Fortunately, I could use Obsidian plugins to save my "Workspaces" (arrangements of panes) and to set up a way to navigate between them with a keyboard shortcut (hotkey).

First, enable the Workspaces plugin, in Core Plugins in Settings. Then, create the two Workspaces. Bring up your search note (`Search Research Notes.md` in my case). Collapse the File Explorer on the left (the list of your files and folders) to create more space for the list of found records. Click on the "Manage workspace layouts" in the left bar (your button may look differently but the description will be the same):

![manage workspace layouts.png](res/manage%20workspace%20layouts.png)  
Type the name of your search workspace (no spaces) in the window that comes up.

![add search layout.png](res/add%20search%20layout.png)

Click save. Now, create your note workspace. Start with File Explorer open and with one pane displaying your note. Click on the three dots in the upper right corner of your note ("More options") and choose "Open local graph". Click on "More options" again and choose "Open backlinks."

![open backlinks.png](res/open%20backlinks.png)

You will end up with three panes open. Now, drag your backlinks pane to the lower right corner.

![drag backlinks.png](res/drag%20backlinks.png)

You should end up with a workspace that includes the File Explorer, your note, a local Graph view for your note, and Backlinks for your note:

![notes workspace.png](res/notes%20workspace.png)  
Click on the "Manage workspace layouts" in the left bar again, type the name for your note workspace ("Work-with-notes" in my case), and save.

### Set Up Workspace Navigation

To quickly switch between your two workspaces while working on the same note, you need to install two more Community Plugins:

- [Advanced URI](https://github.com/Vinzent03/obsidian-advanced-uri) - creates a link to a workspace
- [QuickAdd](https://github.com/chhoumann/quickadd) - runs a script to switch to a workspace

Next, in your javascripts folder (`meta/javascript` in my case) create three files: `workspace-load-Search-research-notes.js`

```
module.exports = async () =>
{
	window.open("obsidian://advanced-uri?vault=my-research&workspace=Search-research-notes");
}
```

... `workspace-load-Work-with-notes.js`

```
module.exports = async () =>
{
	window.open("obsidian://advanced-uri?vault=my-research&workspace=Work-with-notes");
}
```

... and `load-current-note.js`

```
module.exports = async () =>
{
	const text = await navigator.clipboard.readText();
	window.open(window.open(text));
}
```

The first two scripts open a link to a workspace, and the third opens a note with the file path saved to the Clipboard.

Next, open QuickAdd. Now it gets complicated, so I am including a screenshot for every step. On the first screen click on "Manage Macros":

![manage macros.png](res/manage%20macros.png)  
A new window will open. Type the title of your new macro, "Work with Notes" and click on "Add macro" button.

![add work with notes macro.png](res/add%20work%20with%20notes%20macro.png)

Another window will open. Now you have to add a series of steps to open the workspace with the correct note.

First, add a step to copy the URI for the current note with the Advanced URI plugin:

![copy uri for current file.png](res/copy%20uri%20for%20current%20file.png)

Add your own script to open the Work-with-notes workspace:

![user script work with notes.png](res/user%20script%20work%20with%20notes.png)

Add the wait command - to slow down the process so the next script step could load properly (if you have an older computer, and the script doesn't work for you, try increasing the wait time):

![add wait command.png](res/add%20wait%20command.png)

Finally, add your own script for loading the current note:

![user script load current note.png](res/user%20script%20load%20current%20note.png)

The final macro should look like this:

![work with notes entire script.png](res/work%20with%20notes%20entire%20script.png)

Now close the window. In the previous window, you have to add a "Choice": an action that uses the macro you just created. Name it "Work with notes" and choose "Macro" from the pulldown menu.  
![add choice - work with notes macro.png](res/add%20choice%20-%20work%20with%20notes%20macro.png)  
You can click on the lightning sign to add this choice to the top of the Command Palette (optional). Clik on the gear next to the "choice" you just created to configure it.

![configure work with notes choice.png](res/configure%20work%20with%20notes%20choice.png)  
A new window will open. Choose the "Work with notes" macro from the pulldown menu and close this window. You are done with the first action.

![choose work with notes macro.png](res/choose%20work%20with%20notes%20macro.png)  
Repeat the steps to create the Search research notes macro and "choice." One difference: this second macro will only include your user script to open the "Search-research-notes" workspace:

![search research notes macro.png](res/search%20research%20notes%20macro.png)

You have to close and reopen Obsidian for these actions to become active.

You can use the QuickAdd actions from the Command Palette, but it is more convenient to use keyboard shortcuts. Open Hotkeys in Settings and type "quickadd" to bring up the actions. Click on "Customize this command" and type the keys you want to use. I use `Cmd-S` for search and `Cmd-N` for the notes workspace.

![hotkeys for workspaces.png](res/hotkeys%20for%20workspaces.png)  
Now you can easily locate your research notes and navigate between workspaces (keyboard commands appear in the lower left corner of the gif):

![navigate workspaces.gif](res/navigate%20workspaces.gif)

Next step is to link your research notes to your own analysis notes, so you can concentrate on the famous Obsidian feature, writing-via-linking.