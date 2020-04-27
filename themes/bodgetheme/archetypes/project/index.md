---
date        : {{ .Date }}
lastmod     : {{ .Date }}
draft       : true
short_title : "{{ replace .Name "-" " " | title }}"
title       : "{{ replace .Name "-" " " | title }} Project"
description : "This is the project page description for the {{ replace .Name "-" " " | title }} Project."

# Identifying mnemonics, INTERNAL use only.
# This refers to this project from other items like blogs, teams, etc.
projects    : ["{{ replace .Name "-" " " | upper }}"]

# For alternative external reference only
slugs       : ["{{ replace .Name "-" " " | lower }}"]

# Project state
active      : true
archived    : false

# Identifying tags, searchable/visible to site visitors
tags        :
- {{ replace .Name "-" " " | upper }}

# Identifying categories, searchable/visible to site visitors
categories  :
- Hacker conference badge
- Hardware design
- Software development
- Embedded software

# Project icon
# For available icons, see: https://fontawesome.com
icon_name : fa-suitcase
icon_pack : fa

# Default images related to this project
image_src   : "images/mascot.png"
image_alt   : "{{ replace .Name "-" " " | upper }}"
thumb_src   : "images/mascot.png"
thumb_alt   : "{{ replace .Name "-" " " | upper }}"

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

### {{< icon name="fa-suitcase" >}} {{ replace .Name "-" " " | title }} Project

Welcome to the project page of the {{ replace .Name "-" " " | title }} project. This project page is still a work in progress and we expect to fill it with content soon.
{{< img src="/images/wip.png" alt="Work in progress." width="50%"  >}}
