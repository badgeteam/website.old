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
- image   : "image1.jpg"
  caption : "Imagine One"
- image   : "image2.jpg"
  caption : "Imagine Two"
---
