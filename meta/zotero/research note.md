| | |------------ | ------------| | Title | {{title}} | | Authors | {{authors}} | | Publication | {{publicationTitle}} | | Zotero link | {{pdfZoteroLink}} | | Web link | {{url}} |
Citation

{{bibliography}}

{% if abstractNote %}
Abstract

{{abstractNote}}

{% endif %}
Annotations
Exported: {{exportDate | format("YYYY-MM-DD h:mm a")}}

{% for annotation in annotations %} {% if annotation.annotatedText %}

    Highlight {{annotation.annotatedText}} Page {{annotation.page}} {% endif %} {% if annotation.comment %} Comment {{annotation.comment}} Page {{annotation.page}} {% endif %} {% if annotation.imageRelativePath %} ![[{{annotation.imageRelativePath}}]] {% endif %} {% endfor %}

{% persist "notes" %}
Take-aways

Related

Tags

#wip #literature-note #medicin #zotero {% endpersist %}