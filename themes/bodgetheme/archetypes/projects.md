---
date: {{ .Date }}
draft: true
title:  "{{ replace .TranslationBaseName "-" " " | title }}"
description : "{{ replace .TranslationBaseName "-" " " | title }} Project"
tags: []
categories: []
projects: [""{{ replace .TranslationBaseName "-" " " | upper }}""]
image-src : ""
image-alt : "Project"
archived: false
---
