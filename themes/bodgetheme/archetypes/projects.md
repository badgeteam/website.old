---
date        : {{ .Date }}
draft       : true
short_title : "{{ replace .TranslationBaseName "-" " " | title }}"
title       : "{{ replace .TranslationBaseName "-" " " | title }}"
description : "{{ replace .TranslationBaseName "-" " " | title }} Project"
tags        : []
categories  : []
activities  : [""{{ replace .TranslationBaseName "-" " " | upper }}""]
image_src   : ""
image_alt   : "Project"
thumb_src   : ""
thumb_alt   : "Project"
archived    : false
---

Project page content goes here.
