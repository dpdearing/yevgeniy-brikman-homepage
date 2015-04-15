---
layout: post
title: 'Proposal: extend Markdown syntax to support form elements'
date: '2011-07-26T01:03:00.000-07:00'
author: Yevgeniy Brikman
tags:
- Ideas
- Web Development
- Open Source
- Software Engineering
modified_time: '2011-09-07T15:06:53.212-07:00'
thumbnail: http://1.bp.blogspot.com/-PpvqqnAwsxY/Ti5yfzvx0II/AAAAAAAAJtg/6Q7gYkBV8aY/s72-c/markdown.png
blogger_id: tag:blogger.com,1999:blog-5422014336627804072.post-2818022916028139401
blogger_orig_url: http://brikis98.blogspot.com/2011/07/proposal-extend-markdown-syntax-to.html
---

[Markdown](http://daringfireball.net/projects/markdown/) is a lightweight 
markup language that can be converted into HTML. The main inspiration behind 
its syntax is to copy what most people have used for years to decorate plain 
text emails. For example, if you emphasize a word by surrounding it with 
*asterisks*, you get <code>&lt;em&gt;asterisks&lt;/em&gt;</code>. If you try 
to put in a page divider with a bunch of dashes ---------------, you get 
<code>&lt;hr/&gt;</code>. The syntax *visually represents* the type of HTML 
output you desire; in a way, Markdown is the onomatopoeia of markup languages. 

<table align="center" cellpadding="0" cellspacing="0" 
class="tr-caption-container" style="margin-left: auto; margin-right: auto; 
text-align: center;"><td style="text-align: center;">[<img border="0" 
height="62" 
src="http://1.bp.blogspot.com/-PpvqqnAwsxY/Ti5yfzvx0II/AAAAAAAAJtg/6Q7gYkBV8aY/s320/markdown.png" 
width="244" 
/>](http://1.bp.blogspot.com/-PpvqqnAwsxY/Ti5yfzvx0II/AAAAAAAAJtg/6Q7gYkBV8aY/s1600/markdown.png)<td 
class="tr-caption" style="text-align: center;">Markdown was created by [John 
Gruber](http://daringfireball.net/) and [Aaron 
Swartz](http://www.aaronsw.com/) 
Markdown is VERY* *easy to read and write, so it's a great choice for 
[CMS](http://en.wikipedia.org/wiki/Content_management_system), 
[wiki](http://en.wikipedia.org/wiki/Wiki) and 
[WYSIWYG](http://en.wikipedia.org/wiki/WYSIWYG) use cases. 
[GitHub](http://www.github.com/) and 
[StackOverflow](http://www.stackoverflow.com/) both make heavy use of Markdown 
and have created their own Markdown extensions and implementations: [GitHub 
flavored Markdown](http://github.github.com/github-flavored-markdown/) and 
[MarkdownSharp](http://code.google.com/p/markdownsharp/). I too am a fan of 
Markdown: I think it's perfect for formatting answers on StackOverflow, it's a 
slick way to support rich text formatting in [Resume 
Builder](http://resume.linkedinlabs.com/), and in my [open source 
projects](https://github.com/brikis98), it's an elegant solution for readme 
files that are perfectly readable with or without a Markdown interpreter. 

<span style="font-size: large;">**Proposal** 

In this blog post, I'm going to propose a small extension to the Markdown 
syntax: support for forms. There are a number of CMS and wiki use cases where 
I've wanted to allow users to create a custom form (e.g. a simple poll or 
event RSVP) without having to write out the full HTML for it. I even created a 
[github project](https://github.com/brikis98/wmd) (forked from 
[wmd](https://github.com/ChiperSoft/wmd)) to try to implement this extension, 
though I've been too damn busy to get to it. Perhaps someone will be inspired 
by this post and help me get this thing rolling :) 

<span style="font-size: large;">**Syntax** 

## Text fields 

<script src="https://gist.github.com/1106204.js?file=TextBox.text"></script> 
<script src="https://gist.github.com/1106204.js?file=TextBox.html"></script> 

## Radio buttons 

<script 
src="https://gist.github.com/1106204.js?file=RadioButtons.text"></script> 
<script 
src="https://gist.github.com/1106204.js?file=RadioButtons.html"></script> 

## Check boxes 

<script 
src="https://gist.github.com/1106204.js?file=CheckBoxes.text"></script> 
<script 
src="https://gist.github.com/1106204.js?file=CheckBoxes.html"></script> 

## Drop down 

<script src="https://gist.github.com/1106204.js?file=DropDown.text"></script> 
<script src="https://gist.github.com/1106204.js?file=DropDown.html"></script> 

## Required fields 

<script 
src="https://gist.github.com/1106204.js?file=RequiredFields.text"></script> 
<script 
src="https://gist.github.com/1106204.js?file=RequiredFields.html"></script> 

<span style="font-size: large;">**Feedback** 

Hopefully, merely looking at the examples above makes my proposal clear. If 
not, I've clearly failed, as Markdown's central goal is readability. Either 
way, let me know what you think in the comments. Also, feel free to fork my 
[github project](https://github.com/brikis98/wmd) for this proposal and start 
hacking away! 

## Update: [Geoff](https://github.com/maleldil) saw this post, forked my 
project, and [implemented the proposal](https://github.com/maleldil/wmd)! 
Awesome work Geoff! 