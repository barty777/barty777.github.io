---
title: "Kindle notes parser"
layout: post
date: 2017-02-05 21:20
tag:
- kindle
- python
- notes
- highlights
image: /assets/images/projects/kindle/header.jpg"
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: "Post about my Kindle notes parser"
category: project
author: bfreskura
externalLink: false
---

If you're an avid reader like I am, then the Kindle is the best way to
revolutionize your reading life. It has many advantages
over paper books:
* easier to carry than most of the books
* all books are in the one place
* bookstore is just a few clicks away
* you can bookmark, take notes, and make highlights
* reading in the dark is now painless

One problem with Kindle is that your notes and highlights are stored in a
textual file on the device and it is not so easy to display them in a pretty 
format like PDF. This is why I have created this script which can do just that:
parse the notes and highlights data and extract them in multiple formats.
Supported export formats are LaTeX, Markdown and plain text. One nice feature
is that you can create new export templates for any of the supported formats so
you're not limited to the default ones.

<div class="image">
    <img alt="PDF" src="{{ site.baseurl }}/assets/images/projects/kindle/example.jpg" width="500">
    <div class="caption">PDF export example of highlights</div>
</div>

## How to use
The script is written in Python3 and it is started as a Python script:

`python3 export.py --input-log [/My/Clippings/path] --output-dir [/export/directory] --templates-dir [templates/]`

Next, you'll be offered with a list of books which contain any user data. After
selecting the title, you can choose your export format and the export template.

Voilà, you now have the exported files which can easily be converted into PDF or
something that suits your needs.


More information about the script, along with the source code can be found in the official 
[repo](https://github.com/barty777/kindle_note_parser).

