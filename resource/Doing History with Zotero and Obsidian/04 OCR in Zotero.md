![highlighting after ocr.png](res/highlighting%20after%20ocr.png)

Often the documents I get from online databases are not searchable, for example, I cannot search or highlight pages from the _Historical New York Times_. To search and annotate the text, I run OCR (optical character recognition) on these files. Adobe Acrobat is the easiest OCR app to use, but you have to pay a monthly fee and you need to go through extra steps to open your PDF outside of Zotero. Instead, I use [Tesseract](https://github.com/tesseract-ocr/tesseract), a free alternative to Adobe Acrobat that you can run from within Zotero. On balance, Tesseract is [no worse](https://source.opennews.org/articles/so-many-ocr-options/) at OCR than Acrobat or other popular tools.

For this feature, you need to install several components via the command line. Here I show how to install them via the Terminal app on a Mac. If you are a PC user, check out [these instructions](https://www.jdavidstark.com/how-to-extract-text-from-image-only-pdfs-with-zotero/) for Windows.

You will need:

[Zotero OCR](https://github.com/UB-Mannheim/zotero-ocr) plugin (install as you would any Zotero plugin)  
[Homebrew](https://brew.sh/) (command-line, an app that installs the last two apps)  
Tesseract (command-line, install via Homebrew)  
Poppler (command-line, install via Homebrew)

First, download the [Zotero OCR](https://github.com/UB-Mannheim/zotero-ocr) plugin from Github and install in Zotero.

![add zotero ocr.png](res/add%20zotero%20ocr.png)

Open Terminal app. You will see a window with a prompt that will look similar to this:

![terminal window.png](res/terminal%20window.png)

To install [Homebrew](https://brew.sh/), copy this line (without the accent marks) and paste it into the Terminal at the prompt, then press enter:

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

You will see a bunch of lines reporting on the installation. Wait until you see the prompt again. Then install Tesseract...

```
brew install tesseract
```

... and poppler:

```
brew install poppler
```

To get location for Tesseract and pdftoppm (you will need these for Zotero OCR preferences), enter these two commands in the Terminal on a Mac (highlighted in yellow in the picture below):

```
brew list tesseract
```

and

```
brew list poppler
```

In each case you will get a list of files.

![tesseract location.png](res/tesseract%20location.png)

Copy the line that ends with `/tesseract` (in my case, the first line in blue in the picture above). Open Zotero OCR preferences:...

![open zotero ocr preferences.png](res/open%20zotero%20ocr%20preferences.png)

... and add the path. Do the same for the line ending with `/pdftoppm` (in my case, the second line in blue in the picture above). Check "Save output as PDF with text layer" and uncheck everything else.

![zotero ocr preferences.png](res/zotero%20ocr%20preferences.png)

Now find a file that needs OCR (a document you cannot search or highlight). Make sure that the file is not open in the PDF viewer. Run the plugin:

![run ocr.png](res/run%20ocr.png)

Wait for the process to complete. After OCR is complete, the plugin will add a linked PDF to the item (with a slightly different icon):

![linked pdf.png](res/linked%20pdf.png)

Move the original PDF to the Trash (you can still recover it if there is a problem):

![move original pdf to trash.png](res/move%20original%20pdf%20to%20trash.png)

Convert the new linked file to a stored file (in the following dialogue, you can leave the "Delete original file after storing" option unchecked):

![convert linked file to stored file.png](res/convert%20linked%20file%20to%20stored%20file.png)

Now you can open the PDF, and add a highlight:

![open and annotate.gif](res/open%20and%20annotate.gif)

Once you are sure that the new PDF works, you can delete the original PDF by emptying the Trash. All extra files created by Tesseract during OCR will also be deleted in this step.

Congratulations, you are now independent from Adobe and can OCR your documents for free.