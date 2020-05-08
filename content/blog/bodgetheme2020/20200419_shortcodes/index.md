---
date        : 2020-04-19T17:58:57+02:00
lastmod     : 2020-04-25T22:31:57+02:00
draft       : false
title       : "Testing with shortcodes"
author      : "Elborro"

# Description overrides the automated summary of marked-up content
#  at the bottom of this file.
description : ""

# Identifying mnemonics, INTERNAL use only. Fill AT LEAST one identifying
# mnemonic, to refer to the project this blog is related to.
projects    : ["Bodgetheme"]

# External reference name (i.e. https://bodge.theme/blog/slug)
slug        : ""

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
image_src   : ""
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

##### Development tests with shortcodes

<!--more-->

{{< highlight html >}}
{{</* tweet 1224084891559759872 */>}}
{{</ highlight>}}

{{< tweet 1224084891559759872 >}}

{{< highlight html >}}
{{</* tweet-single 1224084891559759872 */>}}
{{</ highlight>}}

{{< tweet-single 1224084891559759872 >}}




{{< highlight html >}}
{{</* tweet 1224084929623023624 */>}}
{{</ highlight>}}

{{< tweet 1224084929623023624 >}}

{{< highlight html >}}
{{</* tweet-single 1224084929623023624 */>}}
{{</ highlight>}}

{{< tweet-single 1224084929623023624 >}}




{{< highlight html >}}
{{</* tweet 1224084963852783620 */>}}
{{</ highlight>}}

{{< tweet 1224084963852783620 >}}

{{< highlight html >}}
{{</* tweet-single 1224084963852783620 */>}}
{{</ highlight>}}

{{< tweet-single 1224084963852783620 >}}
