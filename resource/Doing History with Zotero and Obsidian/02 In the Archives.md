
![twitter question on archives.png](res/twitter%20question%20on%20archives.png)

_Note: All Obsidian plugins, scripts, and settings described here are included in the starter [Obsidian history vault](https://github.com/erazlogo/obsidian-history-vault) available for download on Github. You can also watch a YouTube video, [Doing History with Zotero and Obsidian: Archival Research](https://www.youtube.com/watch?v=i-CJ-SmU7rA)._

Historian [Liz Covart](https://www.lizcovart.com/) recently [asked](https://twitter.com/lizcovart/status/1501629336125771777) a question (above) that comes up every year, because apps and devices useful for archival research improve every few months. These digital tools fall into three rough categories: a device to take pictures, a place to store your photos, and a way to track your research progress.

Your choice should depend on [[01 Notetaking for Historians|how you plan to take notes]] from your documents (Zotero and Obsidian in my case) and on the copying restrictions in the archive you plan to visit. Even if you are working in another app, such as [DevonThink](https://www.devontechnologies.com/apps/devonthink) or [Tropy](https://tropy.org/), your research workflow is likely the same as mine: photograph, store, and keep track. Because I have to work in archives with restrictions on copying (in Russia) I prefer the most portable, fast, and error-proof solution: no tripod or stand, no SLR camera, and only three apps: a smartphone scanner app, Zotero, and Obsidian.

In the best case scenario, at the end of an archival trip I end up with a "saved search" (a collection based on search criteria) in Zotero of all folders I photographed. (Russian archives instead store bound volumes of documents called "archival units" but whatever the designation of your units, the process will be the same.) Each folder item includes archival location information, short description of contents, dates, and attached PDF of scans.

![archival folders.png](res/archival%20folders.png)

Here I explain how to get to this point and what to do when conditions are not ideal.

### What you need

Smartphone + scanner app  
Zotero + Obsidian

### Scan with a Smartphone Scanner App

Before you leave for the archive, make sure your smartphone has extensive free hard drive space and maximum battery charge.

I use an iPhone app to scan documents. Adobe Scan can do that best according to reviews. I use an older program, Scanner Pro because it has more options to frame, size, and color-correct documents once photographed. Whatever app you use, it should have the following features:

1. Ability to focus quickly and reliably. Most apps can do that now within a second. Tap in the middle of the image if you are not sure--that tells the app where to focus.
    
2. Ability to crop the document automatically from the photograph. This is a basic feature of scanner apps that speeds up the process--you don't have to align the shot before taking it.
    
3. Ability to straighten the document. This is also a basic and crucial feature. Whatever angle you use to photograph the page, in the end it will appear as if you made a perfectly aligned shot. This feature may distort the dimensions of the page and the font shape slightly, but it is very fast. These distortions do not matter for OCR or reading. If you want a more precise rendition of the page, you should pre-set the exact size of the page in settings.
    

![scanner app.png](res/scanner%20app.png)

4. Ability to export in jpeg format. Because of above distortions, images (photographs or drawings) on the page may appear in a wrong ratio. If you want to use an image for an illustration later, you need to make a more careful shot and export it separately as a jpeg.
    
5. Ability to export in PDF format. I scan everything from one folder into one "multi-page scan" and name it as follows: archive abbreviation + archive location (box, folder, etc.) + short description of what's in the folder. This makes import into Zotero easier.
    
6. Ability to save to the cloud (extensive hard drive space on your smartphone helps for conditions where wifi or cellular service is not available). Most apps can save to Dropbox or iCloud continuously while you scan. This works reliably for me, so I usually transfer all the folders I scanned to Zotero in the end of the day, instead of doing it after I finish with each folder.
    
7. Ability to OCR before export (optional). This speeds up PDF annotation in Zotero. This is worth it if most of your documents are typed and legible. Small print, handwritten pages, and faint carbon copies of typed documents in most cases will not give you searchable text. I use a free and open source program, Tesseract, and a Zotero OCR plugin to [[04 OCR in Zotero|OCR typed documents after I add them to Zotero]].
    

At the end of each folder, I rename the "multi-page scan" file according to naming conventions above. Then I start a new multi-page scan. And so on until my day in the archive is over.

### Store Scanned Folders as PDFs in Zotero

At the end of the day I export all scanned folders as PDFs to my laptop. I drag all these PDFs into Zotero at once, then select-all, control-click (on a Mac), and choose "Create Parent Items." Because I already named the files as archive+location+description, I end up with recognizable "folder" items in no time.

![create zotero folder items.gif](res/create%20zotero%20folder%20items.gif)  
I add tags: type of source ("primary"+"folder"), project name, and any subject tags as appropriate. To add a tag to all new folder items at once, you need to select them and drag them on top of the tag in the pane on the bottom-left.

I add the year for each folder in the date field, for sorting.

I clean up a bit: delete ".pdf" form the title field and change item type to Manuscript. (Archive/Loc. in Archive fields are available both in Manuscript and Document item types, so you could use the default Document type for folders and not worry about changing to Manuscript. I just prefer Manuscript because its icon visually denotes archival sources.)

In the "Archive" and "Loc. in Archive" fields I enter the information as it should appear in the citation for any document within that folder. I also add language information whenever the language of most documents in the folder is other than English (Russian in my case). (Zotero uses the language field to [prevent title casing of non-English titles](https://www.zotero.org/support/kb/preventing_title_casing_for_non-english_titles) in citations.)

![folder item russian with tags.png](res/folder%20item%20russian%20with%20tags.png)  
Archival collections are cited differently depending on the country or institution of the collection. For example, citations for U.S. archives usually put the archive or library ("depository" for a "manuscript collection" in the [Chicago Manual of Style](https://www.chicagomanualofstyle.org) terminology) last:

> Burton to Merriam, telegram, 26 January 1923, box 26, folder 17, Charles E. Merriam Papers, Special Collections Research Center, University of Chicago Library.

But citations for [Soviet archives](https://www.ucl.ac.uk/ceelbas/understanding-structure-soviet-archives) put the depository first:

> RGALI, f. 1573, op. 5, ed. khr. 242, l. 3.

Because of inconsistent citation rules, Zotero cannot format all of the different cases correctly in the citation. Most likely, you will have to revise the citations manually for publication.

As far as Zotero item fields are concerned, in the above cases,

Location in Archive field would contain:

> **US archives:** box 26, folder 17  
> **Soviet archives:** f. 1573, op. 5, ed. khr. 242

Archive field would contain:

> **US archives:** Charles E. Merriam Papers, Special Collections Research Center, University of Chicago Library  
> **Soviet archives:** Russian State Archive for Literature and Art (RGALI)

For folder items and individual archival documents, I enter abbreviations in the Archive field except in cases when I use only one or two documents from a collection. For US archives, I use collection abbreviations. Because of citation conventions, for Soviet archives I use depository abbreviations (RGALI, for example) and put collection information in the Location in Archive field. Your system should depend on the citation conventions in your field.

To keep track of these abbreviations, I create items tagged "collection" for every collection I intend to examine, with a full name of the collection in the Title field, information about the depository in the Place field, abbreviation in the Short Title field, and the link to the finding aid (if available) in the URL field. You can export these items into an "Archival Collections" section of your bibliography (you'll have to tweak the formatting here as well).

![collection item with tags.png](res/collection%20item%20with%20tags.png)

I put collection abbreviation (JSCL) into the Archive field for each folder item in this collection:

![from collection to folder.png](res/from%20collection%20to%20folder.png)

The "folder" item is my basic unit in Zotero for keeping track of what I scanned. I don't delete these items or any pages in the pdfs as I process the folders further.

To keep my folder items easily accessible, I create a saved search folder for Archive = (collection abbreviation) AND tag = "folder."

![save a search zotero.png](res/save%20a%20search%20zotero.png)

I don't enter everything from the folder as individual items, just sources I know I will cite somewhere and always something that I enter as a research note in Obsidian.

When I need to enter an item for an individual document from the folder--a letter or a report, for example--I just duplicate that folder item (control-click and choose "Duplicate Item") to reproduce archive and location information automatically:

![duplicate item.png](res/duplicate%20item.png)

Then I change the other metadata to reflect the document:

![from folder to document.png](res/from%20folder%20to%20document.png)

I delete the tag "folder" to make sure that my saved search for folders does not include individual items.

I usually export individual document pages as a separate PDF and attach this PDF to the new item. This optional extra step saves time if you know you will need to go back several times to the document for more context.

I cite archival documents with the collection abbreviation in drafts. For publication, I change the first mention of the collection in the work to full citation. For a book or dissertation, you would usually create a list of abbreviations for archival collections.

### Track Your Research with Obsidian

Obsidian comes handy for tracking your research, especially when you can't scan everything. In a dedicated "05 archives" directory in Obsidian, I use notes to track folders I need to look at in various collections. I use tags to mark these notes: [#archive/name-of-archive](https://publish.obsidian.md/#archive/name-of-archive).

For each archive where I can take photos for free, I just have a note with a list of folders with short descriptions of contents, and check folders off as "done" as I view them. In US archives you can usually compile such a list from an online finding aid. But if the archive charges fees for photography or does not allow it, you need to track your research more precisely.

When I have to pay for my photos or request scans for a fee, I add an Obsidian note for each folder. I tag them as [#requested](https://publish.obsidian.md/#requested) from the archive; slated to [#copy](https://publish.obsidian.md/#copy); [#scanned](https://publish.obsidian.md/#scanned); [#in-progress](https://publish.obsidian.md/#in-progress); or [#done](https://publish.obsidian.md/#done) (viewed and transcribed). A note for a useful folder contains a rough table of contents, in case I decide to request a document or two remotely from the archive later on. I also tag the "useless" folders as [#done](https://publish.obsidian.md/#done) and leave a note for myself why I don't need them, so I don't request them later again by mistake. I take photos or request scans of the parts I definitely need.

![archives folder.png](res/archives%20folder.png)

When I can't photograph anything at all, I start by indexing each folder in a new note in the "archives" folder. As I go along, whenever I find a useful document, I record the metadata and a quote or summary.

To make sure I don't forget to create a Zotero item and a research note for each transcribed document, I add a "file document" task to each. (To add a task, I just type `- [ ] your task` on a new line.)

In this Obsidian [#archive](https://publish.obsidian.md/#archive) note, I jotted down a table of contents for relevant sources and transcribed important passages, each marked with a "file document" task. Each note also includes tags for project and archive, as well as an index of relevant people, places, and events. The note title includes archive name and location in the archive:

GARF = State Archive of the Russian Federation

P9518-1-1136 = fond P9518 (collection), opis 1 (sub-collection); ed. khr. 1136 ("archival unit").

![archives note with transcribed source.png](res/archives%20note%20with%20transcribed%20source.png)

To track all unprocessed transcribed documents, I rely on Obsidian [Dataview](https://github.com/blacksmithgu/obsidian-dataview) plugin. [[01 Notetaking for Historians#Zotero Integration Setup|I explain how to install Obsidian plugins elsewhere]]. Dataview can search for fields, links, and tasks.

I create a separate note that has nothing but this code:

````

``` dataview
TASK FROM "05 archives"
WHERE text="file document"
```
````

As a result, I get a list of links to all unprocessed documents:

![file document task list.png](res/file%20document%20task%20list.png)  
At some point later, I enter the metadata for each transcribed document into Zotero (here also, you can duplicate an item to copy archive and location information from one item to the next). I extract the text of each document (or summary) to a new [[01 Notetaking for Historians|research note]] in Obsidian linked to its Zotero item. Then I delete the relevant task. And so on, until there is nothing left to process.

### Archival Research at a Glance

Here is my archival research process in one chart:

![archival research.png](res/archival%20research.png)

Now all that's left to do is [[01 Notetaking for Historians|annotate documents and create research notes]].