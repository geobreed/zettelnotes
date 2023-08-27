If your research process requires you to link from a Zotero item back to related notes in Obsidian, you need the [Mark-DB-Connect](https://github.com/daeh/zotero-markdb-connect) plugin. This plugin requires BetterBibTex citekeys included in the YAML section of your notes. It also requires that all your notes linked to Zotero items reside in one folder ("01 notes" in my case). You may also want to keep only notes with a valid Zotero BibTex citekey in this folder, otherwise you'll get error notices from the plugin every time you sync.

To configure the plugin, open settings:

![open citations plugin settings.png](res/open%20citations%20plugin%20settings.png)

You need to change the following: set the folder containing notes; choose the “Custom File Filter” radio button and change the custom file filter to `.+\.md$`; select "Match notes based on BetterBibTex citekey" and set yaml keyword to "citekey".

![citation plugin first screen.png](res/citation%20plugin%20first%20screen.png)

On the next screen, if you have several Obsidian vaults, select the Obsidian vault name that will open the notes.

![citation plugin second screen.png](res/citation%20plugin%20second%20screen.png)

I assign a color (blue) to the tag used by the plugin to distinguish the items with reference notes in a list view.

![assign tag color.gif](res/assign%20tag%20color.gif)

I also create a "saved search" (a collection based on search criteria) by this tag that contains all my items that have research notes associated with them.

Now you just need to run the plugin:

![run citation plugin.png](res/run%20citation%20plugin.png)

Now you can connect from Zotero back to the research note:

![zotero to obsidian.gif](res/zotero%20to%20obsidian.gif)