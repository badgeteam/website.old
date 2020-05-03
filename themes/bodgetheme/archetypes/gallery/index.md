---
date        : {{ .Date }}
draft       : true
title       : "{{ replace .Name "-" " " | title }}"

# Identifying tags, searchable/visible to site visitors
tags        :
- "Gallery"
- "{{ replace .Name "-" " " | upper }}"

# Identifying categories, searchable/visible to site visitors
categories  :
- "Gallery"

# Photo gallery
gallery:
- album   : "images"
  exclude : false
  images  :
  - image        : "imagine.jpg"
    caption      : "Imagine"
    exclude      : false
    external_url : ""
  - image        : "people.jpg"
    caption      : "People"
    exclude      : false
    external_url : ""
---
