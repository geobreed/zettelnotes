
![write with pandoc.jpeg](res/write%20with%20pandoc.jpeg)  
_Note: Obsidian plugins, scripts, and settings described here are NOT YET included in the starter [Obsidian history vault](https://github.com/erazlogo/obsidian-history-vault) available for download on Github. I will get to that eventually. You have to install the Pandoc app yourself as well._

As the above [post](https://discord.com/channels/686053708261228577/722584061087842365/1007841108501483530) on Obsidian Discord suggests, the question of writing in Obsidian often comes up. I used to write in Word, then Scrivener, then Ulysses, gradually moving from complex to stripped-down options and from rich text to markdown. Now I write in Obsidian. I use [Pandoc](https://pandoc.org/) to cite-as-you-write. I just finished a chapter entirely in Obsidian and the setup worked just fine. Because the setup is a bit complicated, I first explain my work process. If you find it useful, you can go to the following sections to get installation and options instructions.

### Work process - Workspace

My writing workspace looks like this:

![writing workspace.png](res/writing%20workspace.png)

This workspace is organized as follows:

- On the left, a pane with an analysis note that articulates my argument and links to research notes, and a left-bottom pane with a local graph in case I need to follow the links.
- At the bottom, the corkboard with links to key notes for the chapter and to search interfaces that will help me to find any other notes I need. You can also use it for tasks or anything else related to the project.
- In the middle, the writing space where I work on a paragraph that will go into the chapter. The width of this pane matches the "readable line length" setting in Obsidian.
- On the right, the outline where I sort my paragraphs in the correct order.

I also use the left pane for searching notes. And the right pane I also use for displaying the bibliography of all sources cited in the current paragraph, with the [Pandoc Reference List](https://github.com/mgmeyers/obsidian-pandoc-reference-list) plugin.

![search bibliography hover.png](res/search%20bibliography%20hover.png)  
The citation in the brackets is a [BibTex citekey](https://retorque.re/zotero-better-bibtex/citing/) generated in Zotero. By hovering over it I can see the full reference.

These features allow me to stay within the same interface while I write: I can search my notes, follow the graph links for linked notes, sort my paragraphs into an article, add citations, and display my bibliography on the fly.

### Work Process - Composing and Export

For a new piece of writing, I first create a folder for my draft within my writing folder, `03 writing`--for example, "X blog post" or "Y chapter." Then control-click on the folder and mark it as a [Longform](https://github.com/kevboh/longform) project.

![mark as longform project.png](res/mark%20as%20longform%20project.png)

This command creates Drafts subfolder and Index file for keeping my paragraphs ordered (see above). Then I press `Ctrl-L` to get to the writing view. To start my first paragraph, I just type the main point of the paragraph in at the bottom of the right column, in the "New Scene" field, and hit enter to create a new note. The Longform plugin was created for writing fiction, so the term "scene" refers to a scene from a novel or a nonfiction magazine article, but it is really just a note, for my purposes a paragraph, that can be sorted into an outline.

![new scene.png](res/new%20scene.png)  
I create separate notes for the article title and the subsection titles and title them in caps so my list of paragraphs becomes an outline. You can move the paragraphs around to put them in the correct order:

![move scenes.png](res/move%20scenes.png)

To find a research note that may be helpful for the paragraph I am writing, I use the search feature in the Kanban board (first I make sure the left pane is active, then I click on the search link). Or, I may follow the link from a note I just found:

![search and graph for writing.gif](res/search%20and%20graph%20for%20writing.gif)

To add Pandoc citations from Zotero I use [Zotero Integration](https://github.com/mgmeyers/obsidian-zotero-integration). I pull up a Zotero search strip with a shortcut `Shift-Command-2`, type words from author and title, and hit enter. I end up with a citation or several, and I enclose them in square brackets, for example, `[@gioiaHound1989; redman2022]`. (If you want to add comments to the citations, such as "see also," make sure to add them in the end or the beginning. If you add comments in between citations, your export will be broken.)

![find citation.png](res/find%20citation.png)  
To add a footnote, I use the `Shift-Command-6` shortcut. If you are using a footnote style, Pandoc will make footnotes out of the references you entered. But if you are using a parenthetical style, you may need a manual footnote for a comment. Obviously, any footnotes I add in a given note will start with number 1. I renumber them when I compile the entire manuscript

To check my writing for style and flow, I switch to the Reading view and see the paragraph without these citations.

![hide references.gif](res/hide%20references.gif)  
If I want to focus on editing a paragraph, I hit `Option-Command-Shift-Z` to enter the focus mode. I enter `Option-Command-Z` to exit:

![focus mode.gif](res/focus%20mode.gif)

When I am done writing my first draft, I compile it using the basic template in Longform. I exclude note titles. This helps if you don't want to name your article sections in the final draft but want to know what they are while you are writing. This also means that my article title and section titles have to be in the body of the note to make it into the draft. Longform will open the compiled manuscript in the new pane.

![compile manuscript.png](res/compile%20manuscript.png)  
To renumber footnotes, I click on the three dots in the upper right corner of the manuscript pane, and choose "Lint file" from the options list. This command keeps the order of the footnotes, not their numbers (for example, the link to footnote number two in the paragraph will work even if it is positioned before footnote number 1 at the bottom of the text. But "Lint file" command will break that connection.)

Next, I export the compiled manuscript to Word with the `Shift-Command-W` shortcut.

![export manuscript.gif](res/export%20manuscript.gif)

Below I only explain how to set up the plugins necessary for writing. Elsewhere on this site, you can read instructions on how to set up [[03 Search Research Notes#Set Up Workspaces|workspaces]], [[03 Search Research Notes#Set Up Workspace Navigation|workspace navigation]], and [[03 Search Research Notes#Set Up the Search Page and Script|search]] pages.

### Install Pandoc

Pandoc allows you to convert your markdown text into a Microsoft Word file with citations in the format of your choice and a bibliography attached at the end. Install the Pandoc app from an [installer](https://pandoc.org/installing.html) file available on the Pandoc site. This is straightforward.

### Export Citations from Zotero into a JSON text file

In order to export your text into a Microsoft Word file with formatted citations and a bibliography, you need a JSON (JavaScript Object Notation) version of your Zotero references. This also allows you to view bibliographic references while you are writing up a paragraph (see image above).

First, make sure you have BetterBibTex Zotero plugin installed via xpi. BetterBibTex also has an option to export as a .bib file, but only the .json option will export the archival information (box, folder, etc.), so for historians .json is necessary.

Create a folder in Obsidian for the bibliography (in my case, `meta/bibtex`). Then go to Zotero, control-click on your collection or saved search, and choose, Export collection" or "Export saved search." (You can also export your entire library. My library is very large, so I prefer to export by folder.)

![export saved search.png](res/export%20saved%20search.png)  
I organize my bibliographies as saved searches by project, and export those saved searches. With this option, each source I tag with the `free-music-project` tag is automatically added to the folder. I have to re-export the bibliography manually to keep it updated in Obsidian, but it is more important to me to keep my Zotero bibliography up to date via tags.

If you keep your bibliography in a regular Zotero collection, you can set the BetterBibTex plugin to automatically update your .json file--just check "Keep updated" in the next dialogue, along with "Background export." Choose "Better CSL JSON" as the format.

![bibliography export options.png](res/bibliography%20export%20options.png)  
Save the file as something you can remember (in my case, `free-music-project.json`).

### Install Plugins

In Zotero, you need only the Better BibTex plugin installed via xpi.

In Obsidian, you will need the following plugins installed in the Community Plugins section in Settings:

- Zotero Integration
- Longform
- Obsidian Pandoc plugin
- Pandoc Reference List
- Obsidian Footnotes
- Linter
- Focus Mode

### Configure the Pandoc Plugin

The Pandoc plugin exports your text into a Microsoft Word file with formatted citations and a bibliography. Set the Pandoc Plugin settings as follows:

![pandoc settings.png](res/pandoc%20settings.png)

- In the section "Export files from HTML or markdown?" choose "Markdown."
- Set Export folder -- full path to either Downloads or Desktop folder.
- Extra Pandoc arguments--copy text above but include two of your own variables:
    - Choose the full path to the .json file you just exported into Zotero. It will depend on the location of your Obsidian vault folder (in my case the path is `/Users/er/obsidian/my-research/meta/bibtex/free-music-project.json`)
    - Choose the full path to a csl file you want to use for your export at the moment. In the image below, the style I set is Chicago Author-Date. The full path to the file will be in the `styles` folder within your Zotero folder (in my case, `Users/er/zotero/styles/chicago-author-date.csl`).
- Set Pandoc path to the current location for Pandoc app on your computer. This is a bit complicated. You might need to find the path in the Terminal:

Open Terminal app. You will see a window with a prompt that will look similar to this:

![terminal window.png](res/terminal%20window.png)

To find the path to Pandoc app, copy this line (without the accent marks) and paste it into the Terminal at the prompt, then press enter:

```
which pandoc
```

Whatever you get back should go into the Pandoc path preference (in my case, it is `/usr/local/bin/pandoc`).

Set a shortcut for export to Word in Hotkeys in Obsidian Settings (`Shift-Command-W` recommended).

![hotkey for export to word.png](res/hotkey%20for%20export%20to%20word.png)

### Configure Pandoc Reference Plugin

Pandoc Reference Plugin allows you to view full references for all citations while you are writing up a paragraph. It is also necessary if you want to hide your citations in the Reading view. The preferences are as follows:

![pandoc plugin preferences.png](res/pandoc%20plugin%20preferences.png)

- Path to bibliography file - the full path to the .json file you just exported into Zotero (same as in the Pandoc Plugin)
- Path to CSL file - the full path to a .csl file you want to use for viewing the references. I prefer the Chicago Full Note Style for that, so my path is `Users/er/zotero/styles/chicago-full-note.csl`.
- Fallback Path to Pandoc - same as the Pandoc path preference in the Pandoc plugin
- Hide links - On
- Show Citekey Tooltips - On

### Add CSS Snippet to Hide Citations

This snippet by [Chris Grieser](https://github.com/chrisgrieser) allows you to proofread your paragraphs without the distractions of in-text citations. It only works when the Pandoc Reference Plugin is installed and activated.

Open the "snippets" folder in `your-vault/.obsidian/snippets` (on a Mac, first press `Shift-Cmd-.` to make hidden folders visible).

Create a text file called `hidecitations.css` and place it in the `snippets` folder:

```
.markdown-preview-view :is(.pandoc-citation, .pandoc-citation-extra, .pandoc-citation-formatting) {
  display: none;
}
```

Now go to Settings -> Appearance and activate the snippet.

![activate hidecitations snippet.png](res/activate%20hidecitations%20snippet.png)

### Configure Other Plugins

You don't need to configure Longform further unless you want to add steps to the Compile function. Settings contain one feature you may want to use, however: you can "untrack all projects" if you start having problems with them. This only happens when you rename folders.

Set a shortcut for manual footnotes in Hotkeys in Obsidian Preferences (`Shift-Command-6` recommended).

![hotkey for footnotes.png](res/hotkey%20for%20footnotes.png)  
Linter has many useful preferences, but for writing you only need to activate "Move Footnotes to the bottom" and "Re-index Footnotes."

![linter preferences.png](res/linter%20preferences.png)

Happy writing!