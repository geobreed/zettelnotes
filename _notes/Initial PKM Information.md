---
title: Initial PKM Information
date: 20221023
tags:
---

# How To Setup This Site
This is going to be a super simple post about how to setup and use this theme for your own website.

### Setup Prerequisites

For this tutorial, we’ll need to install a few things on your machine (you may have some of these already). Following the instructions on each website to install them.

- [[Ruby::https://www.ruby-lang.org/]]
- [[RubyGems::https://rubygems.org/]]
- [[Git::https://git-scm.com/downloads]]

You’ll also need to create accounts on the following services:

- [[GitHub::https://www.github.com/join]] (to store the website)
- [[Netlify::https://app.netlify.com/signup]] (to serve the website so others can see)

Once you are all set with the prerequisites, we can then get to the fun part of getting it to appear on your screen. Let's get started with that.

### 1. Create a fork of the template repository

To simplify things, I provide the template showed in the image above to get started. You can always tweak this template to your taste later.

Visit the GitHub page for my template repository [[Maxence-L/notenote.link::https://github.com/Maxence-L/notenote.link]], and fork it to your account using the Fork button:

> <img src="/assets/img/fork_button.jpg" style="box-shadow: 2px 2px 20px 0 #ddd;"/>

Once the forking process is complete, you should have a fork (essentially a copy) of my template in your own GitHub account. On the GitHub page for your repository, click on the green “Clone or download” button, and copy the URL: we’ll need it for the next step.

### 2. Clone your repository locally 

Next, we want to download the files from your GitHub repository onto your local machine. To do this, replace <YOUR_COPIED_URL_HERE> in the command below with the URL you copied in the previous step, then execute this command:

```
$ git clone <YOUR_COPIED_URL_HERE> my-personal-website
```

As a reference point, this is how it looks like for me (the difference is likely just the GitHub username):

```
$ git clone git@github.com/Maxence-L/notenote.link my-personal-website
```

Then, navigate into the directory that was just created:

```
$ cd my-personal-website
```

### 3. Test out the site locally

Sweet! You now have your repository’s source code on your machine. Within the my-personal-website directory, run the following command to install the necessary dependencies like Jekyll:

```
$ bundle
```

Once that’s done, ask Jekyll to start serving the site locally:

```
$ bundle exec jekyll serve
```

Then, open up [[http://localhost:4000::http://localhost:4000]] in your browser.

If everything’s done correctly, you should now see the home page of your Personal Jekyll Website with notenote.link Theme. 🎉

Keep in mind that this site is only available locally (notice the `localhost` part of the URL), so if we want it to be available on the Internet for everyone to enjoy, we need to deploy it to the Internet: we’ll use Netlify for that in the next step.

### 4. Connect your GitHub repository to Netlify

Netlify lets you automatically deploy your personal website on to the Internet when you update your GitHub repository. To do this, we need to connect your GitHub repository to Netlify:

1. Log in to Netlify
2. Once logged in, click the “New site from Git” button
3. On the next page, select GitHub as the continuous deployment provider (you may need to authorize the connection, in which case, approve it)
4. On the next page, select your website repository from the list.
5. On the next page, replace the basic build settings with the following.
    1. Type in "jekyll build" (without the quotes) inside the text field titled "Build Command".
    2. Similarly type in "_site/" (without the quotes) inside the text field titled "Publish Directory".
6. On the next page, keep the default settings, and click on “Deploy site”.

That was easy! We’re almost done.

Wait a couple of minutes for the initial deploy to complete.

Once that’s done, your website should be available on the Internet via a generic Netlify URL, which you can change to a custom domain later if you’d like.

Now the cool thing is this: whenever you push an update to your GitHub repository, Netlify will automatically deploy your updates to the Internet.

### 5. Start producing content :

At this point, you can start updating the files on your machine (in the my-personal-website folder) to change your jekyll seamless based website to your liking: update the copy, add some notes, tweak the layout, customize the colors, etc. Once you have something you’re happy with, push your changes to your GitHub repository with the following commands:

```
$ git add --all
$ git commit -m 'Update content'
$ git push origin master
```

If that command succeeds and the rest of the tutorial was done correctly, in a couple of minutes, you should see your changes live on your Netlify website. 🚀

And we’re done! You now have your own notenote.link based Personal Website .


# How to use the special feature
## The default features

All the default jekyll markdown features are made available such that they don't cause any conflict with the custom features that we have implemented. 

Internal links (simple and with alt-text) and LateX delimiters in markdown are compatible with [[Obsidian::https://obsidian.md]]. I'd recommend using it as a CMS for managing your notes. See the page about Obsidian integration below for more details.

To see how to the raw markdown gets generated, go to the [[Test page to see how the raw markdown is rendered]]

## The Custom features

### 1. Creating a wiki-style link

**<u>General Syntax</u>**

- **Internal links:** **[​[**​Some Link**]]**

- **Internal links with alternative text:** **[​[**​Some Link\\|Alt text**]]**

- **External links:** **[​[​**Some Text::https://address-to-the-website**]]**

Anything text inside a double square bracket is considered as an internal link. The text has to be a valid title, if you provide a random text inside double square brackets, it will showup highlighted in yellow telling you that there is no essay/article/file with the mentioned title.

Similarly, for external links all you have to do is add a double colon after the "Alt text" and enter the link to the website after the double colon as seen below.

**Examples**

Example of an internal link that points to a valid post or page, that is, a page with the title (not url) mentioned in the double brackets.

> **Raw Syntax:** **[​[**​Obsidian integration**]]**
>
> **Rendered Text:** Obsidian integration


Example of an internal link that do not point to a valid post or page, that is, a page with the title (not url) mentioned in the double brackets.

> **Raw Syntax:** **[​[**Title of a non-existent page**]]**
> 
> **Rendered Text:** Title of a non-existent page

### 2. Creating a sidenote or a marginnote

**<u>General Syntax</u>**

- **Sidenote:** **[​[**Some Text**::keyword-of-the-type-of-the-sidenote]]**

- **Marginnote:** **[​[​**Some Text**::keyword-of-the-type-of-the-marginnote]]**

> |Type of the sidenote/marginnote|keyword|
  |:--|:--|
  |Left Sidenote| `lsn` |
  |Right Sidenote | `rsn` |
  |Left Marginnote| `lmn` |
  |Right Marginnote | `rmn` |


So, all you have to do is type in the keywords of the corresponding type of sidenote or marginnote after the double colon in the above syntax

**Examples**

Example of a sidenote to the right side of the page: 

> **Raw Syntax:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec rutrum tortor in pharetra vehicula. Fusce gravida lacus ac sem luctus congue at id justo. Ut sed tempus ante. **[​[**Phasellus mollis lectus id efficitur mollis.**::rsn]]** Suspendisse sit amet diam nec justo rhoncus tristique. Ut blandit faucibus nisi vitae rutrum. Vivamus fermentum efficitur justo non facilisis.
>
> **Rendered Text:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec rutrum tortor in pharetra vehicula. Fusce gravida lacus ac sem luctus congue at id justo. Ut sed tempus ante. [[Phasellus mollis lectus id efficitur mollis.::rsn]] Suspendisse sit amet diam nec justo rhoncus tristique. Ut blandit faucibus nisi vitae rutrum. Vivamus fermentum efficitur justo non facilisis.

Same goes with `lsn`, `rmn`, `lmn`

### 3. Highlighting a piece of text

**<u>General Syntax</u>**

- **[​[**​Some Link**::highlight]]**

There is only one color right now in which it highlights, a light bluish color, but you can easily extend it to support multiple colors by tinkering with it in `content.html` file in `_includes` directory.

**Examples**

> **Raw Syntax:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec rutrum tortor in pharetra vehicula. Fusce gravida lacus ac sem luctus congue at id justo. Ut sed tempus ante. **[​[**Phasellus mollis lectus id efficitur mollis.**::highlight]]** Suspendisse sit amet diam nec justo rhoncus tristique. Ut blandit faucibus nisi vitae rutrum. Vivamus fermentum efficitur justo non facilisis.
>
> **Rendered Text:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec rutrum tortor in pharetra vehicula. Fusce gravida lacus ac sem luctus congue at id justo. Ut sed tempus ante. [[Phasellus mollis lectus id efficitur mollis.::highlight]] Suspendisse sit amet diam nec justo rhoncus tristique. Ut blandit faucibus nisi vitae rutrum. Vivamus fermentum efficitur justo non facilisis.

### 4. Partial Transclusion

Transclusion is just a natural extension of sidenote and marginnote feature.

**<u>General Syntax</u>**

- **Sidenote-transclusion:** **[​[**Some Text**::keyword-of-the-type-of-the-sidenote-transclusion]]**

- **Marginnote-transclusion:** **[​[​**Some Text**::keyword-of-the-type-of-the-marginnote-transclusion]]**

> |Type of the sidenote/marginnote transclusion|keyword|
  |:--|:--|
  |Left Sidenote Transclusion | `lsn-transclude` |
  |Right Sidenote Transclusion | `rsn-transclude` |
  |Left Marginnote Transclusion | `lmn-transclude` |
  |Right Marginnote Transclusion | `rmn-transclude` |


So, all you have to do is type in the keywords of the corresponding type of sidenote or marginnote after the double colon in the above syntax

**Examples**

Example of a transclusion to the right side of the page: 

> **Raw Syntax:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec rutrum tortor in pharetra vehicula. Fusce gravida lacus ac sem luctus congue at id justo. Ut sed tempus ante. **[​[**Obsidian integration**::rmn-transclude]]** Suspendisse sit amet diam nec justo rhoncus tristique. Ut blandit faucibus nisi vitae rutrum. Vivamus fermentum efficitur justo non facilisis.
>
> **Rendered Text:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec rutrum tortor in pharetra vehicula. Fusce gravida lacus ac sem luctus congue at id justo. Ut sed tempus ante. [[Obsidian integration::rmn-transclude]] Suspendisse sit amet diam nec justo rhoncus tristique. Ut blandit faucibus nisi vitae rutrum. Vivamus fermentum efficitur justo non facilisis.

Same goes with `rsn`, `lsn`, `lmn`

### 5. Wrapping a text inside a box

**<u>General Syntax</u>**

- **[​[**Some Text**::wrap]]**

**Examples**

> **Raw Syntax:** **[​[**Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec rutrum tortor in pharetra vehicula. Fusce gravida lacus ac sem luctus congue at id justo. Ut sed tempus ante. Suspendisse sit amet diam nec justo rhoncus tristique. Ut blandit faucibus nisi vitae rutrum. Vivamus fermentum efficitur justo non facilisis**::wrap]]**.
>
> **Rendered Text:** [[Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec rutrum tortor in pharetra vehicula. Fusce gravida lacus ac sem luctus congue at id justo. Ut sed tempus ante. Suspendisse sit amet diam nec justo rhoncus tristique. Ut blandit faucibus nisi vitae rutrum. Vivamus fermentum efficitur justo non facilisis.::wrap]]

### 6. Flashcard

**<u>General Syntax</u>**

- **[​[**Some Text**::srs]]**

**Examples**

> **Raw Syntax:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. **[​[**Donec rutrum tortor in pharetra vehicula**::srs]]**. Fusce gravida lacus ac sem luctus congue at id justo. Ut sed tempus ante. Suspendisse sit amet diam nec justo rhoncus tristique. Ut blandit faucibus nisi vitae rutrum. Vivamus fermentum efficitur justo non facilisis.
>
> **Rendered Text:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. [[Donec rutrum tortor in pharetra vehicula::srs]]. Fusce gravida lacus ac sem luctus congue at id justo. Ut sed tempus ante. Suspendisse sit amet diam nec justo rhoncus tristique. Ut blandit faucibus nisi vitae rutrum. Vivamus fermentum efficitur justo non facilisis.

### 7. Specific classes for changing font-type, font-size, and font-weight

There are classes like very-small, medium-small, small, small-medium, medium, medium-large, large, very-large; that can be used to change the size of your text directly from markdown like this:

> **Raw Syntax:**
> {:.regular-sans}
> ```
> {:.large}
> Some text here that needs to be enlarged
> ```
>
> **Rendered Text:**
> 
> {:.large}
> Some text here that needs to be enlarged


Similarly there are classes like regular-sans, serif, bold, italic, oblique, bolder, etc for formatting the text.

> **Raw Syntax:**
> 
> ```
> {:.medium .serif .oblique}
> Some text here that needs to be enlarged
> ```
>
> **Rendered Text:**
> 
> {:.medium .serif .oblique}
> Some text here that needs to be enlarged

Other common classes are .boxit that is used to wrap the text, .disable-user-select to disallow users from being able to select a particular piece of text by selecting it, etc. There are more classes like these which you can see in the file `style.css`. Once you figure out which class to use, all you have to do is just add the class before the text you want inside a curl brace like this ​{:\<classnames-with-dot-prepended-to-them>​}

### 8. Table of Content

notenote.link supports automatic table of content (toc) generation. Just add a `toc: true` line in the front matter at the beginning of your post.

You can modify the maximum header level included in the toc by changing number in the following option in `config.yml` :
```
toc:
  max_level: 3
```

### 9. Note maturity
Since this jekyll theme aims at mirroring your Obsidian notebook, the note content may note be mature or complete yet.

Therefore, we use front matter to classify the notes in the following categories (in order of appearance in the front page feed) : 

- `season: summer` : the note is near-complete (more than 80% done)
- `season: spring` : the note is in progress and has already good content
- `season: winter` : the note has just started, a summary is present however.
- `season: automn` : the note needs refactoring or some rewriting. It won't appear in the front-page feed.

Why use seasons ? Since this theme is a form of 'digital garden', I thought it would make sense to keep the analogy.

### 10. Other implicit features.

Features like backlinks, context menu, related posts, page preview are available by default as they are implemented using CSS and JS. So, you don't have to do anything other than write as you would normally to make use of those features.

# Obsidian Integration
## Obsidian Integration
The main purpose of this fork, other than cosmetic changes, is to create a web representation of an [[Obsidian::https://obsidian.md]] vault, using the [[Simply-Jekyll::https://github.com/raghuveerdotnet/simply-jekyll]] template.z

### Usage

Things to know :

- Markdown is fully-compatible (including Latex delimiters !)

- There are now only notes (no blog posts). If you really want blog posts along notes, a hack is to set the YAML season of blog posts to `summer` and notes to `automn` - they won't appear in feed but will be searchable and appear in tags page.

- Code is now correctly indented

- You can change the code template by replacing the css in `/assets/css/highlight.css` by any template from [[pygment.css::https://github.com/richleland/pygments-css]]

- Wikilinks are usable : **[​[**​...**]]**,

- Also alt-text wikilinks (with transclusion !) : **[​[**​original link\\|alternative text**]]**

Please note : You need to escape the pipe character in Obsidian (\\| instead of \|). This won't break Obsidian's functionality.

- **Fresh new feature** : you can also link headers ! Use # when typing the wikilink : **[​[**Obsidian integration#Obsidian setup\|Alt-text**]]** will create the link with "Alt-text" text link (click on it to see the effect)

Please note : This feature will work only if you write alternative text in the link : "Obsidian integration#Obsidian" setup won't work[^1]. 

[^1]: I don't use it, so I didn't change it but if it's important for you open an issue and I may fix it.

- You can use [[Simply-Jekyll custom features::https://simply-jekyll.netlify.app/posts/exploring-the-features-of-simply-jekyll]], such as flashcards : [[flashcards !::srs]] - but don't click on it in Obsidian, else it will create a new page.

### Obsidian setup

#### Installation
After having forked [[notenote.link::https://github.com/Maxence-L/notenote.link]] on your computer, open Obsidian and create a vault in the root folder (`/notenote.link`).

This will allow you to modify all your markdown files inside the directory. 

`about.md` is in the root folder.

Your notes should go to the `_notes` folder, images in `assets/img`. You need to tell Obsidian where to put the new notes. In Preferences/File, enter the following settings :

![](/assets/img/new%20notes%20pref.png#center)

- Default location for new notes : In the folder specified below`
- Folder to create new notes in : `_notes`
- New link format : `Relative Path to file`
- Attachment folder path : `assets/img

### Frontmatter

Front matter is needed at the beginning of your note. Here is the template :

```YAML
---
title: My Note
tags: tag1
toc: true
season: winter
---
```

You can hide it in Obsidian by toggling the option "Show Frontmatter" in the Preferences/Editor menu.

#### Images

Images are the tricky part : 

- You can use vanilla markdown links: `![](/asset/img/img.png)`
- You can drag/drop/paste images in Obsidian, which will create a link such as : `[​[​../assets/img/Pasted image.png]]`

A quick hack in the last case is just to change the brackets : `![](../assets/img/Pasted image.png)`

