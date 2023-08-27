Some annotations I import are citations or bibliography entries: anything in footnotes or bibliography of my source that belongs in my Zotero database. Down the road, I need to process these differently from my research notes: add them to Zotero.

But I don't always have time to do that right away. Everything I need to do in the future I file in the "04 tasks" folder in Obsidian. I mark all notes in the folder with the [#task](https://publish.obsidian.md/#task) tag.

I use Templater for extracting references for my task note in the same way I [[01 Notetaking for Historians#Processing Imported Annotations|extract research notes]].

In the "meta/templater" folder, place "extract bibliography task from selection.md" file with this text:

```
<%*
tp.file.create_new('#task \n'+tp.user.projecttag(tp)+'\n\n'+ tp.file.selection(), "new task");
-%>
```

In the "meta/javascript" folder, place "projecttag.js" with this text:

```
function projecttag(tp) {
	string = tp.file.tags.filter((tag) => tag.includes("#project")).join("\n");
    return string;
}
module.exports = projecttag
```

Set up keyboard shortcuts in Settings. I chose Cmd-T as the hotkey.

Now, you can select any text in your note imported from Zotero and press the Cmd-T hotkey. The new note will have the text you selected preceded by tags: [#task](https://publish.obsidian.md/#task) and a project tag from the original note.

![extract task note.gif](res/extract%20task%20note.gif)

As you can see, I [[Option - Configure Zotero to Categorize Your Annotations|configured Zotero]] to add a note to myself to "enter reference" for each of these annotations.