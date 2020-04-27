---
date        : 2020-04-06T14:21:02+01:00
draft       : false
title       : "Blogpage images"
author      : "Elborro"
description : "While standard formatting should deliver quite a clean page, someone might want to add images at a later stage."

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
image_src   : "images/bodgeteam.jpg"
image_alt   : "Bodgenators"
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

## Inserting images in text

### Use the following shortcode to insert an image

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg" alt="Bodgenators" width="50%" descr="Description." */>}}
{{</ highlight>}}

### Or formatted like a card

{{< highlight html >}}
{{</* img-card src="images/bodgeteam.jpg" alt="Bodgenators" width="50%" descr="Description." */>}}
{{</ highlight>}}

{{< note >}}Note that **src** is a only mandatory parameter.{{< /note >}}

----

### Insert image - 100% width, including description

{{< img src="images/bodgeteam.jpg" alt="Bodgenators" descr="Let's show a quite long description to see if this gets nice wrapped onto the next line and such." >}}

----

### Insert image - 50% width, including description

{{< img src="images/bodgeteam.jpg" alt="Bodgenators" width="50%" descr="Let's show a quite long description to see if this gets nice wrapped onto the next line and such." >}}

----

### Insert image-card - 50% width

{{< img-card src="images/bodgeteam.jpg" alt="Bodgenators" width="50%" >}}

----

### Insert image-card - 50% width, description

{{< img-card src="images/bodgeteam.jpg" alt="Bodgenators" width="50%" descr="Let's show a quite long description to see if this gets nice wrapped onto the next line and such." >}}

----

### Insert image-card - 50% width, title

{{< img-card src="images/bodgeteam.jpg" alt="Bodgenators" width="50%" title="Bodgenators" >}}

----

### Insert image-card - 50% width, title and description

{{< img-card src="images/bodgeteam.jpg" alt="Bodgenators" width="50%" title="Bodgenators" descr="Let's show a quite long description to see if this gets nice wrapped onto the next line and such." >}}

----

### Insert image - 100% width

{{< img src="images/bodgeteam.jpg" alt="Bodgenators" >}}

----

### Insert image - 100% width, title

{{< img src="images/bodgeteam.jpg" alt="Bodgenators" title="Bodgenators" >}}

----

### Insert image - 100% width, description

{{< img src="images/bodgeteam.jpg" alt="Bodgenators" descr="Let's show a quite long description to see if this gets nice wrapped onto the next line and such." >}}

----

### Insert image - 100% width, title and description

{{< img src="images/bodgeteam.jpg" alt="Bodgenators" title="Bodgenators" descr="Let's show a quite long description to see if this gets nice wrapped onto the next line and such." >}}
