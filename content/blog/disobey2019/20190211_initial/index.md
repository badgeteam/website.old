---
date        : 2019-02-11T19:56:02+01:00
draft       : false
title       : "Disobey 2019 badge"
author      : "annejan"
description : "Disobey 2019 badge"

# At least one Identifying mnemonic, referring to the project(s) his blog is related to
projects    : ["DISOBEY2019"]

# Identifying tags, searchable/visible to site visitors
tags        :
- Badge
- Disobey2019
- Disobey
- 2019

# Identifying categories, searchable/visible to site visitors
categories  : []

# Blog icon
icon_name : fa-pencil
icon_pack : fa

# Default image related to this blog
image_src   : "images/badge.jpg"
image_alt   : "Disobey 2019"
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
  - image   : "disobey2019.jpg"
    caption : "Disobey 2019"
    exclude : false
  - image   : "badge.jpg"
    caption : "Disobey 2019"
    exclude : false
- album   : "thumbs"
  exclude : true
  images  :
  - image   : "disobey2019.png"
    caption : "Disobey 2019"
    exclude : false
---

# Hardware

- 128x64 pixel LCD
- SAMD ?!
- IR io
- ?!

# Startup guide to Disobey badge
Below is a short introduction to the badge. Please read!

Arriving at Disobey2019, you have likely received a custom PCB badge to accompany the event. There are multiple badge types to differentiate event-goers from staff and people somehow involved with the event. Each badge takes 2x AAA alkaline 1.5V batteries. If you need to replace them, please use the same type.

When you get the badge, make sure you put in batteries and start it up first time at the venue. The badge will need to update its software via "badge" wireless network. It will require manual re-flashing, if it does not succeed in fetching the firmware through the venue wifi!

Badge can be accessed from the computer via USB. It communicates via serial at 115200 baudrate. In Linux it should appear as /dev/ttyACM0 (or at first free number, higher than 0). You can open the Menu and navigate it, or invoke MicroPython shell and live-code on the hardware!

Badge also offers an on-screen menu. You can trigger manually an OTA firmware update, change default WiFi credentials (especially usefull after the event, when you use it at home!).

You can develop code for the badge directly on it via serial connection. You can connect to the Hatchery server and download applications other have uploaded there, and run them on your badge. You can develop your own applications and upload them as MicroPython eggs to Hatchery! (Since Disobey badge is using SHA-2017 MicroPython with modifications, you can also access public SHA-2017 hatchery and see, and maybe even run their apps!)

There is a [guide to the API of MicroPython](https://wiki.badge.team/Disobey2019Badge/API "MicroPython") available on the badge.

Slides of [badge talk](doc/Disobey_talk.pdf "Presentation").
