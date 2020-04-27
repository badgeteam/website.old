---
date        : 2020-04-04T09:24:02+01:00
draft       : false
title       : "Blogpage formatting - built in shortcodes"
author      : "Elborro"
description : "Testing Hugo built in shortcodes (and check for requirement to replace any)."

# Description overrides the automated summary of marked-up content
#  at the bottom of this file.
description : ""

# Identifying mnemonics, INTERNAL use only. Fill AT LEAST one identifying
# mnemonic, to refer to the project this blog is related to.
projects    : ["Bodgetheme"]

# For alternative external reference only
slugs       : ["bt", "bodgetheme"]

# Identifying tags, searchable/visible to site visitors
tags        :
- website
- Bodgetheme
- 2020

# Identifying categories, searchable/visible to site visitors
categories  :
- Website design

# Blog icon
icon_name : fa-pencil
icon_pack : fa

# Default image related to this blog
image_src   : "images/hh2019.jpg"
image_alt   : ""
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

## Built in Shortcodes

----

### Highlighting code

{{< highlight html >}}
{{</* highlight html */>}}
{{</*/* [Abs Link]({{< ref "gallery/general/index.md" >}}) */*/>}}
{{</* highlight */>}}
{{</ highlight>}}

{{< highlight html >}}
{{</* [Abs Link]({{< ref "gallery/general/index.md" >}}) */>}}
{{</ highlight>}}

----

### Absolute reference

{{< highlight html >}}
{{</* [Abs Link]({{< ref "gallery/general/index.md" >}}) */>}}
{{</ highlight>}}

[Abs Link]({{< ref "gallery/general/index.md" >}})

----

### Relative reference

{{< highlight html >}}
{{</* [Rel Link]({{< relref "gallery/general/index.md" >}}) */>}}
{{</ highlight>}}

[Rel Link]({{< relref "gallery/general/index.md" >}})

----

### Instagram

{{< highlight html >}}
{{</* instagram BWNjjyYFxVx */>}}
{{</ highlight>}}

{{< instagram BWNjjyYFxVx >}}

----

### Instagram without caption

{{< highlight html >}}
{{</* instagram BWNjjyYFxVx hidecaption */>}}
{{</ highlight>}}

{{< instagram BWNjjyYFxVx hidecaption >}}

----

### Twitter

{{< highlight html >}}
{{</* tweet 877500564405444608 */>}}
{{</ highlight>}}

{{< tweet 877500564405444608 >}}

----

### Vimeo

{{< highlight html >}}
{{</* vimeo 146022717 */>}}
{{</ highlight>}}

{{< vimeo 146022717 >}}

----

### Youtube

{{< highlight html >}}
{{</* youtube hu3tAjLaBWw */>}}
{{</ highlight>}}

{{< highlight html >}}
{{</* youtube id="hu3tAjLaBWw" autoplay="true" */>}}
{{</ highlight>}}

{{< youtube hu3tAjLaBWw >}}
