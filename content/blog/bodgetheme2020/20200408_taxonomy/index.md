---
date        : 2020-04-08T23:29:02+01:00
draft       : false
title       : "Taxonomy tests"
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

Taxonomies allow to inventory all teammembers, projects in progress, etc. Test for taxonomies and related shortcodes to display them in blog posts. Just a simplified overview for now. Polishing can be done later.

<!--more-->

#### List teams
{{< list-teams >}}

#### List projects
{{< list-projects >}}

#### List categories
{{< list-categories >}}

#### List tags
{{< list-tags >}}

#### Tag cloud
{{< taxo-cloud >}}
