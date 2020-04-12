---
date        : {{ .Date }}
draft       : true
short_title : "{{ replace .Name "-" " " | title }}"
title       : "{{ replace .Name "-" " " | title }}"
description : "{{ replace .Name "-" " " | title }} Project"

# Identifying mnemonics, to refer to this project from other items like blogs, etc.
projects    : ["{{ replace .Name "-" " " | upper }}"]

# Project state
active      : true
archived    : false

# Identifying tags, searchable/visible to site visitors
tags        :
- {{ replace .Name "-" " " | upper }}

# Identifying categories, searchable/visible to site visitors
categories  : []

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
