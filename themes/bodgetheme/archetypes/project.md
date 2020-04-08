---
date        : {{ .Date }}
draft       : true
short_title : "{{ replace .TranslationBaseName "-" " " | title }}"
title       : "{{ replace .TranslationBaseName "-" " " | title }}"
description : "{{ replace .TranslationBaseName "-" " " | title }} Project"

# Identifying mnemonics, to refer to this project from other items like blogs, etc.
projects    : ["{{ replace .TranslationBaseName "-" " " | upper }}"]

# Identifying tags, searchable/visible to site visitors
tags        :
- {{ replace .TranslationBaseName "-" " " | upper }}

categories  : []

image_src   : ""
image_alt   : "Project"
thumb_src   : ""
thumb_alt   : "Project"
archived    : false
---
