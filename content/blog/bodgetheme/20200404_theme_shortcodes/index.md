---
date        : 2020-04-04T10:31:02+01:00
draft       : false
title       : "Bodgetheme shortcodes"
author      : "Elborro"
description : "Testing additional Bodgetheme shortcodes."

# At least one Identifying mnemonic, referring to the project(s) his blog is related to
projects    : ["Bodgetheme"]

# Identifying tags, searchable/visible to site visitors
tags        :
- Website
- Bodgetheme
- 2020

# Identifying categories, searchable/visible to site visitors
categories  : []

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

## Additional Bodgetheme shortcodes

### External Hyperlink (extref)

{{< highlight html >}}
{{</* {{< extref "https://badge.team">}}Badge.team{{< /extref >}} */>}}
{{</ highlight>}}

{{< extref "https://badge.team">}}Badge.team{{< /extref >}}

----

### External Hyperlink new window (extref)

{{< highlight html >}}
{{</* {{< extref "https://badge.team" 0>}}Badge.team new window{{< /extref >}} */>}}
{{</ highlight>}}

{{< extref "https://badge.team" 0>}}Badge.team new window{{< /extref >}}

----

### Highlighted content (hl)

{{< highlight html >}}
{{</* {{< hl color="blue" >}}Highlighted content.{{< /hl >}} */>}}
{{</ highlight>}}

{{< hl color="blue" >}}Highlighted content.{{< /hl >}}

----

### Note (note)

{{< highlight html >}}
{{</* {{< note >}}This is a note{{< /note >}} */>}}
{{</ highlight>}}

{{< note >}}This is a note{{< /note >}}

----

### Note with title (note)

{{< highlight html >}}
{{</* {{< note "Note" >}}This is a note{{< /note >}} */>}}
{{</ highlight>}}

{{< note "Note" >}}This is a note{{< /note >}}

----

### Alert (alert)

{{< highlight html >}}
{{</* {{< alert >}}This is a generic alert!{{< /alert >}} */>}}
{{</ highlight>}}

{{< alert >}}This is a generic alert!{{< /alert >}}

----

### Alert with title (alert)

{{< highlight html >}}
{{</* {{< alert title="Generic" >}}This is a generic alert!{{< /alert >}} */>}}
{{</ highlight>}}

{{< alert title="Generic" >}}This is a generic alert!{{< /alert >}}

----

### Alert (alert-success)

{{< highlight html >}}
{{</* {{< alert-success >}}Successful test!{{< /alert-success >}} */>}}
{{</ highlight>}}

{{< alert-success >}}Successful test!{{< /alert-success >}}

----

### Alert with title (alert-success)

{{< highlight html >}}
{{</* {{< alert-success "Success" >}}Successful test!{{< /alert-success >}} */>}}
{{</ highlight>}}

{{< alert-success "Success" >}}Successful test!{{< /alert-success >}}

----

### Alert (alert-attention)

{{< highlight html >}}
{{</* {{< alert-attention >}}This is an attention alert{{< /alert-attention >}} */>}}
{{</ highlight>}}

{{< alert-attention >}}This is an attention alert{{< /alert-attention >}}

----

### Alert with title (alert-attention)

{{< highlight html >}}
{{</* {{< alert-attention "Attention" >}}This is an attention alert{{< /alert-attention >}} */>}}
{{</ highlight>}}

{{< alert-attention "Attention" >}}This is an attention alert{{< /alert-attention >}}

----

### Alert (alert-danger)

{{< highlight html >}}
{{</* {{< alert-danger >}}This is a red alert!{{< /alert-danger >}} */>}}
{{</ highlight>}}

{{< alert-danger >}}This is a red alert!{{< /alert-danger >}}

----

### Alert with title (alert-danger)

{{< highlight html >}}
{{</* {{< alert-danger "Dangerous" >}}This is a red alert!{{< /alert-danger >}} */>}}
{{</ highlight>}}

{{< alert-danger "Dangerous" >}}This is a red alert!{{< /alert-danger >}}
