---
date        : 2020-03-16T18:42:02+01:00
draft       : false
title       : "Blogpage formatting - markdown"
author      : "Elborro"
description : "Markdown formatting tests."

# At least one Identifying mnemonic, referring to the project(s) his blog is related to
projects    : ["Bodgetheme"]

# For alternative external reference only
slugs       : ["bt", "bodgetheme"]

# Identifying tags, searchable/visible to site visitors
tags        :
- Website
- Bodgetheme
- 2020

# Identifying categories, searchable/visible to site visitors
categories  : []

# Blog icon
icon_name : fa-pencil
icon_pack : fa

# Default image related to this blog
image_src   : "images/sha2017.jpg"
image_alt   : "Hackerbar"
thumb_src   : ""
thumb_alt   : ""

# Author about box
about_show   : true
about_inline : true

# Photo gallery
gallery:
- album   : "images"
  exclude : true
  images  :
  - image   : "imagine.jpg"
    caption : "Imagine"
    exclude : false
  - image   : "people.jpg"
    caption : "People"
    exclude : false
---

# Testing Markdown

# h1
## h2
### h3
#### h4

#tag

* List 1
+ List 2
- List 3
  - Sublist 1
  + Sublist 2
    + Subsublist 1

1. Numbered List
2. Numbered List
   1. Numbered list

### Lines
----
****

### Typography

*Italics*

**Bold**

***Bold+Italics***

_Italics_

__Bold__

___Bold+Italics___

this_is_not_emphasis

~~Strikethough~~

Content with a -- (dash) and a --- (long dash).

> Block quote

[link](http://link/path/to/target)

[link](http://link/path/to/target "TITLE ON LINK")

[Shared Links with footnotes][target 1]

[Second shared link][target 1]

[target 1]

[target 1]: http://footnote.com

Sample inline code `a++` can be specified here.

![Alt Text](/path/to/image "Optional Tooltip")

----

Copyright: &copy;

Registered: &reg;

Trademark: &trade;

Less than: &lt;

Greater than: &gt;

Ampersand: &amp;

Smiley: &#x1F604;

----

### Table

   Name | Job
--------|------
   Alex | Web Developer
    Bob | Sys Admin
  Gabby | Technical Writer

### Alternate Table

|  Name | Mantra |
|  ---  |   ---  |
| Alex  | There must be a better way. |
| Bob   | Play it safe. |
| Gabby | Try everything, but do what you like. |

----

### Task list

Acme Website task list
- [x] Get the home page up
- [x] Update Privacy Policy and Terms of Use
- [ ] Add the about page
- [ ] Start the blog
- [ ] Enable contact us

----

### Code block

```js
var x= 10;
x++;
console.log(x);
```

----

## Direct Emojis Smile please :smile:

[https://www.webfx.com/tools/emoji-cheat-sheet/](https://www.webfx.com/tools/emoji-cheat-sheet/)

I :heart: Hugo

Wink :wink:

----

## Fractions

1/2

100/999

Not a Number/5

----

## Definition Lists

Alex
: Hippy Web Developer
: Technophile

Bob
: Classic SysAdmin
: Conservative

Gabby
: Cool Content Master
: Cautious

----
