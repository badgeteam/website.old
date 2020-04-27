---
date        : {{ .Date }}
lastmod     : {{ .Date }}
draft       : true
title       : "{{ replace .Name "-" " " | title }}"
author      : "Anonymous"
description : ""

# At least one Identifying mnemonic, referring to the project(s) his blog is related to
projects    : ["ReplaceThisWithTheCorrectProjectID"]

# For alternative external reference only
slugs       : []

# Identifying tags, searchable/visible to site visitors
tags        : []

# Identifying categories, searchable/visible to site visitors
categories  : []

# Blog icon
icon_name : fa-pencil
icon_pack : fa

# Default image related to this blog
image_src   : "images/mascot.png"
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

Welcome to the project page of the {{ replace .Name "-" " " | title }} project. This project page is still a work in progress and we expect to fill it with content soon.
