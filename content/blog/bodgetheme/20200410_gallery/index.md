---
date        : 2020-04-10T12:59:04+01:00
draft       : false
title       : "Gallery test"
author      : "Elborro"
description : "Testing gallery shortcode implementation"

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
image_src   : "images/voyage-cambodge.jpg"
image_alt   : "Cambodge"
thumb_src   : ""
thumb_alt   : ""

# Author about box
about_show   : true
about_inline : true

# Photo gallery
gallery:
- image   : "bodge00.jpeg"
  caption : "Tweak"
  exclude : false
- image   : "bodge01.jpg"
  caption : "Wire"
  exclude : false
- image   : "bodge02.jpg"
  caption : "Bodged"
  exclude : false
- image   : "voyage-cambodge.jpg"
  caption : "Cambodge"
  exclude : false
---

{{< gallery >}}
