# Markdown-Format-Tricks

Table of Contents
=================

  * [Markdown-Format-Tricks](#markdown-format-tricks)
    * [Additing ToC (Table of Content)](#additing-toc-table-of-content)
      * [References](#references)
    * [Embedding image](#embedding-image)
    * [Emoji cheat sheet](#emoji-cheat-sheet)
    * [How to attach a file into readme.md?](#how-to-attach-a-file-into-readmemd)
    * [Gradle task check if property is defined](#gradle-task-check-if-property-is-defined)

Created by [gh-md-toc](https://github.com/ekalinin/github-markdown-toc)

Aiming to make markdown format more fun and viewer friendly, the project addresses topics about the addition of ToC (Table of Content), embedded image and emoji.

## Additing ToC (Table of Contents)
"A ToC (Table of Contents) for README.md shall be handy", I believe most of md file's creators will come across the same question. Indeed, especially for long, multiple pages md file.<br/><br/>
:thumbsup: The <a href="https://github.com/ekalinin/github-markdown-toc">github-markdown-toc.sh</a> is a handy tool doing such conversion.<br/><br/> 
Note: Due to the problem of "-o" under gitbash, we have to temporarily place the downloaded _gh-md-toc.sh_ under _/home/spenserk/README.md_toc_conv_ of machine _sdcvd-wdtfapp01.bom.gov.au_.
The simple procedure using the tool is:
   1. Find a way to transfer the tool to machine, such as _sdcvd-wdtfapp01_
   1. Find a way to transfer the md file to above mentioned machine. (Currently it's under /home/spenserk/README.md_toc_conv)
   1. Log into that machine and change to directorty accommodating the md file, then execute following command at above mentioned directory:   
      _gh-md-toc.sh README.md >toc_
   1. Prefix README.md with resulatnt toc file, followed by necessary manual intervention. To make the conversion stremlined, in other word, avoid manual intervention with guidance in mind that avoid following things in heading in order to be able to be converted to clickable item in ToC:   
      * No '*' is appearing in heading of in order to be converted to a clickable ToC content
      * No '.', such as README.md", appearing in heading in order to be converted to a clickable ToC content 
      * No anchored link is appearing in heading of in order to be converted to a clickable ToC content
   1. Transfer the ToC-headed README.md back to gitlab project directory for rendering 

The effect is self-evident as seen in this page.

### References
* https://github.com/ekalinin/github-markdown-toc
* http://assemble.io/docs/Cheatsheet-Markdown.html
* https://en.wikipedia.org/wiki/Markdown
* https://guides.github.com/features/mastering-markdown/
* http://daringfireball.net/projects/markdown/syntax
* https://github.com/gitlabhq/gitlabhq/blob/master/doc/markdown/markdown.md
   
## Embedding image
   Simply use <img> that is already available of HTML tags.<br/>
   Syntax: _&lt;img src="full or partial path to images file"&gt;_<br/>
   Example: logo of North Melbourne Football Club<br/> <img src="image/nmfc-logo.jpg" alt="logo of North Melbourne Football Club">
## Emoji cheat sheet  
   * http://emoji.codes/
   
## How to attach a file into readme.md?
   * http://stackoverflow.com/questions/10189356/how-to-add-screenshot-to-readmes-in-github-repository

## Gradle task check if property is defined 
   * http://stackoverflow.com/questions/31302232/gradle-task-check-if-property-is-defined   
