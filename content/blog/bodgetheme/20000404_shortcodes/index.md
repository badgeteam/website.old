---
date        : 2000-04-04T13:37:02+01:00
draft       : true
title       : "Blogpage formatting - shortcodes"
author      : "Elborro"
description : "Testing shortcodes."
tags        : []
categories  : []
projects    : ["Bodgetheme"]
image_src   : "images/hh2019.jpg"
image_alt   : "Camping"
---

# Built in Shortcodes

----

### Youtube
{{< youtube hu3tAjLaBWw >}}

----

### Highlighting
{{< highlight html "linenos=table,hl_lines=2, linenostart=1">}}
<!-- Youtube markdown that generates code below -->
{{</* youtube hu3tAjLaBWw */>}}

<!-- Start generated Youtube shortcode -->
{{< youtube hu3tAjLaBWw >}}
<!-- End generated Youtube shortcode -->
{{</ highlight>}}


----

# Additional Bodgetheme shortcodes

### Hyperlink
{{< ref "https://badge.team">}}Badge.team{{< /ref >}}

### Hyperlink new window
{{< ref "https://badge.team" 0>}}Badge.team new window{{< /ref >}}

### Highlighted content
{{< hl color="blue" >}}Highlighted content.{{< /hl >}}

{{< note >}}This is a note{{< /note >}}
{{< note "Note" >}}This is a note{{< /note >}}

{{< alert-success >}}Successful test!{{< /alert-success >}}
{{< alert-success "Success" >}}Successful test!{{< /alert-success >}}

{{< alert-attention >}}This is an attention alert{{< /alert-attention >}}
{{< alert-attention "Attention" >}}This is an attention alert{{< /alert-attention >}}

{{< alert-danger >}}This is a red alert!{{< /alert-danger >}}
{{< alert-danger "Dangerous" >}}This is a red alert!{{< /alert-danger >}}

{{< alert >}}This is a generic alert!{{< /alert >}}
{{< alert title="Generic" >}}This is a generic alert!{{< /alert >}}

----

## List projects
{{< list-projects >}}

## List categories
{{< list-categories >}}

## List tags
{{< list-tags >}}

## Tag cloud
{{< tag-cloud >}}
