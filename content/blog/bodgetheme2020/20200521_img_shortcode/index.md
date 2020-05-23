---
date        : 2020-05-21T19:08:17+02:00
lastmod     : 2020-05-23T15:01:42+02:00
draft       : false
title       : "New img shortcode for blogpage images"
author      : "Elborro"

# Description overrides the automated summary of marked-up content
#  at the bottom of this file.
description : ""

# Identifying mnemonics, INTERNAL use only. Fill AT LEAST one identifying
# mnemonic, to refer to the project this blog is related to.
projects    : ["Bodgetheme"]

# External reference name (i.e. https://bodge.theme/blog/slug)
slug        : ""

# Identifying tags, searchable/visible to site visitors
tags        : []

# Identifying categories, searchable/visible to site visitors
categories  :
- Hacker conference badge
- Hardware design
- Software development
- Embedded software

# Blog icon
# For available icons, see: https://forkaweso.me
icon_name : fa-bug
icon_pack : fa

# Default image related to this blog
image_src   : "images/imgshortcode.png"
#image_alt   : ""
#thumb_src   : ""
#thumb_alt   : ""

# Author about box
about_show   : true
about_inline : true

# Photo gallery
gallery:
- album   : "images"
  exclude : true
  images  :
  - image        : "bodgeteam.jpg"
    caption      : "Bodge Team Heroes"
    alternative  : "Bodge Team Heroes"
    exclude      : false
    external_url : ""
  - image        : "mascot.png"
    caption      : "Bodge Team on the move"
    alternative  : "Bodge Team on the move"
    exclude      : true
    external_url : ""

# Write the content of this blog page below in markup language.
# An emoji cheat sheet can be found here:
#  https://www.webfx.com/tools/emoji-cheat-sheet/
---

While standard formatting should deliver quite a clean page, someone might want to add images at a later stage. This shows how to share nice pictures in your blog-posts.

<!--more-->
---

## The 'img'-shortcode

### Unnamed / positional parameters

{{< highlight html >}}
{{</* img "images/bodgeteam.jpg" */>}}
{{</ highlight>}}

The shortcode will automatically fill to default size (250x250), lookup any meta information found in this blogs gallery-structure to for instance display a title or add a reference to an external larger image.

{{< img "images/bodgeteam.jpg" >}}

---

So, the following line:

{{< highlight html >}}
{{</* img "images/bodgeteam.jpg" "resize" */>}}
{{</ highlight>}}

Resizes the image at default ratio 250x250:

{{< img "images/bodgeteam.jpg" "resize" >}}

---

To specify a different ratio, for instance 500x400:

{{< highlight html >}}
{{</* img "images/bodgeteam.jpg" "resize" "500x400" */>}}
{{</ highlight>}}

{{< img "images/bodgeteam.jpg" "resize" "500x400" >}}

The three parameters given in the examples above, can only be given in this order. The ratio should be always in a third position, hence previous parameters can not be left out. These are the only three parameters that can be passed to the shortcode without name.

---

### Named parameters

You can only specify other options using named parameters, which unfortunately cannot be mixed with positional/unnamed parameters. So, you can either specify what you want using the three parameters shown above, or specify *everything* with named parameters.

Note: You can specify the *named* parameters in any order you like them to be.

The named equivalents of the examples mentioned above are:

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg" */>}}
{{</ highlight>}}

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg" method="resize" */>}}
{{</ highlight>}}

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg" method="resize" size="500x400" */>}}
{{</ highlight>}}

---

All parameters that can be set are, but besides src are all optional:

1. src - source or sources of images
2. method - method used to scale image(s)
3. size - image dimensions.
4. album - source album.
5. alt - alt name or names.
6. caption - caption of the image, or captions of the images.
7. capcol - caption colour.
8. cappos - caption position.
9. title - title or titles.
10. align - alignment in document.
11. colour - background colour.
12. ipcmds - additional image processing commands.
13. option - behavioural commands (overrides).

---

#### 1. Source (src)

The image or images you want to show. When specifying multiple, separate them with a comma.

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg,images/mascot.png" */>}}
{{</ highlight>}}

{{< img src="images/bodgeteam.jpg,images/mascot.png" colour="#ffffff" >}}

Since other parameters were not specified, the images are *filled* to a *250x250* ratio.

{{< note >}}This parameter is mandatory unless you specify an entire album.{{< /note >}}

---

#### 2. Method (method)

When not specified, the shortcode will use *Fill* for all images.

##### **Resize**
Resize with width of 500px and preserve ratio. Specify size as "500x" for width 500px and preserve ratio or "x500" for height 500px and preserve ratio. "500x500" will squeeze the image to fit.

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg,images/mascot.png" method="resize" */>}}
{{</ highlight>}}

{{< img src="images/bodgeteam.jpg,images/mascot.png" method="resize" colour="#ffffff" >}}

##### **Fit**
Scales down the image while preserving the ratio, until it fits either specified height or width. Specifying size as "500x" or "x500" will estimate the other dimension preserving the current ratio.

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg,images/mascot.png" method="fit" */>}}
{{</ highlight>}}

{{< img src="images/bodgeteam.jpg,images/mascot.png" method="fit" colour="#ffffff" >}}

##### **Fill**
Resizes and crops the image to match both given dimensions. Specifying size as "500x" or "x500" will estimate the other dimension preserving the current ratio.

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg,images/mascot.png" method="fill" */>}}
{{</ highlight>}}

{{< img src="images/bodgeteam.jpg,images/mascot.png" method="fill" colour="#ffffff" >}}

##### **None**
Skips image processing and show original image. This disables background colour and the generation of coloured tiles for missing pictures.

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg,images/mascot.png" method="none" */>}}
{{</ highlight>}}

{{< img src="images/bodgeteam.jpg,images/mascot.png" method="none" colour="#ffffff" >}}

The default image processing method is 'fill'.

---

#### 3. Dimensions (size)

If not defined, the default size is set to *250x250* (WxH) for all images.

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg,images/mascot.png" */>}}
{{</ highlight>}}

{{< img src="images/bodgeteam.jpg,images/mascot.png" method="fill" colour="#ffffff" >}}

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg,images/mascot.png" size="100x100" */>}}
{{</ highlight>}}

{{< img src="images/bodgeteam.jpg,images/mascot.png" size="100x100" method="fill" colour="#ffffff" >}}

{{< highlight html >}}
{{</* img src="images/bodgeteam.jpg,images/mascot.png" size="400x400" */>}}
{{</ highlight>}}

{{< img src="images/bodgeteam.jpg,images/mascot.png" size="400x400" method="fill" colour="#ffffff" >}}

---

#### 4. Album (album)

Allows you to specify the source album of the images, as an alternative to specifying these for each image separately in the src-parameter. This allows for shorter src's, but with caveat that this allows the use of images from one album at a time only.

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" colour="#ffffff" >}}

A special case is where you want to show the entire content of the album, _as specified in front matter_.

{{< highlight html >}}
{{</* img album="images" */>}}
{{</ highlight>}}

{{< img album="images" colour="#ffffff" >}}

{{< note >}}It is important to note that some images can be left out by configuring them as excluded in the blogs front matter. In this case one of the images has been excluded automatically.{{< /note >}}

---

#### 5. Alternative text (alt)

Value for the alternative text that will be shown by browser when the picture cannot be found, and used by other type of readers like braille-readers for instance.

Specify just one value for all images or specify multiple values separated by comma. When less values are specified than images, the provided list will be used on rotation.

Unless an option suppresses the use of alt entirely, when alt has not been specified as a parameter, an attempt will be made to lookup a reference to this image in the gallery's front matter. On match the alternative description will be used, or the caption when the alternative is empty or does not exist. If all else fails, the alt-attribute will show the filename of the image.

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" alt="Black and white Badge.Team image with first A corrected to O in red.,Grey badger and golden snek." */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" alt="Black and white Badge.Team image with first A corrected to O in red.,Grey badger and golden snek." colour="#ffffff" >}}

{{< note >}}In this example the alt-text is copied into the title as well. Hover over the images to show the result.{{< /note >}}

---

#### 6. Caption (caption)

Value for the caption text for each picture. Specify just one value for all images or specify multiple values separated by comma. When less values are specified than images, the provided list will be used on rotation.

Unless an option suppresses the use of caption entirely, when caption has not been specified as a parameter, an attempt will be made to lookup a reference to this image in the gallery's front matter. If all else fails, the caption will show the filename of the image.

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" caption="First A corrected to O in red,Grey badger and golden snek" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" caption="First A corrected to O in red,Grey badger and golden snek" colour="#ffffff" >}}

---

#### 7. Caption colour (capcol)

Caption colours can be either specified by name or by colour code.

##### Named colours

A limited number of named colours are specified as text only values.

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" capcol="red" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" capcol="red" colour="#ffffff" >}}

{{< note >}}Current recognized named colours are: amber, aqua, black, blue, blue-grey, brown, cyan, dark-grey, deep-orange, deep-purple, green, grey, indigo, khaki, light-blue, light-green, light-grey, lime, orange, pale-blue, pale-green, pale-red, pale-yellow, pink, purple, red, sand, teal, white and yellow.{{< /note >}}

{{< alert >}}When not recognized, please check the list above for existence and correct spelling.{{< /alert >}}

##### Colour codes

Colour codes are preceded by a hash mark (#) and then three or six hexadecimals.

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" capcol="#b31280" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" capcol="#b31280" colour="#ffffff" >}}

{{< note >}}Example colours can be found on sites like [Color Hex](https://www.color-hex.com/color-palettes/).{{< /note >}}

---

#### 8. Caption position (cappos)

Change the position of the caption



{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" caption="Cap1,Cap2" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" caption="Cap1,Cap2" colour="#ffffff" >}}

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" caption="Cap1,Cap2" cappos="topleft" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" caption="Cap1,Cap2" cappos="topleft" colour="#ffffff" >}}

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" caption="Cap1,Cap2" cappos="bottommiddle" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" caption="Cap1,Cap2" cappos="bottommiddle" colour="#ffffff" >}}

{{< note >}}Current recognized position names are: topleft, topmiddle, topright, left, middle, right, bottomleft, bottommiddle, bottomright and bottom. Where most do place the caption on the image, bottom will place the caption back under it, which is the default as well.{{< /note >}}

{{< alert >}}When not recognized, please check the list above for existence and correct spelling.{{< /alert >}}

---

#### 9. Image title (title)

Value for the title text shown on hover over a picture. Specify just one value for all images or specify multiple values separated by comma. When less values are specified than images, the provided list will be used on rotation.

Unless an option suppresses the use of title entirely, when title is not specified the alt-text will be used.

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" title="Surprise! :)" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" title="Surprise! :)" colour="#ffffff" >}}

{{< note >}}Hover over image to see the result.{{< /note >}}

---

#### 10. Alignment (align)

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" align="left" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png"  align="left" colour="#ffffff" >}}


{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" align="right" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png"  align="right" colour="#ffffff" >}}

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" align="center" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png"  align="center" colour="#ffffff" >}}

---

#### 11. Background colour / fill colour (colour)

The background / fill colour is used to create tiles when the image cannot be found, or to change the background colour on transparent images.

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" colour="#ffffff" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" colour="#ffffff" >}}

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png,unknown.jpg" colour="#b31280" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png,unknown.jpg" colour="#b31280" >}}

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png,unknown.jpg" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png,unknown.jpg" >}}

{{< note >}}Not specifying the colour, forces the shortcode to use the standard site configuration to determine which colour to use.{{< /note >}}

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,unknown01.jpg,mascot.png,unknown02.jpg,unknown03.jpg,unknown04.jpg" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,unknown01.jpg,mascot.png,unknown02.jpg,unknown03.jpg,unknown04.jpg" >}}

{{< note >}}Correct! In previous examples colour="#ffffff" was sneakily added to each example to avoid confusion about colours while explaining a different feature.{{< /note >}}

---

#### 12. Image processing commands (ipcmds)

This feature allows to add additional commands to the Hugo image processor. Please be *very* carefull, since these commands will be fed to the processor *without validation*, it can potentially break and stop the site build process.

Available commands are documented at [Hugo Image Processing](https://gohugo.io/content-management/image-processing/#readout)

{{< alert >}}When using this feature, be sure to ***test and confirm*** proper function ***before*** uploading your blog post for publication!{{< /alert >}}

---

#### 13. Options (option)

Option allows to pass behavioural instructions to the shortcode. For instance to surpress captions completely.

Currently the following options are available:

1. nocaption - Don't show a caption.
2. noalternative - Don't add an alt-attribute.
3. notitle - Don't add a (hoverable) title.
4. nourl - Don't provide a link to an (external) image.

Multiple instructions are separated by comma's.

{{< highlight html >}}
{{</* img album="images" src="bodgeteam.jpg,mascot.png" option="nocap,nourl" */>}}
{{</ highlight>}}

{{< img album="images" src="bodgeteam.jpg,mascot.png" option="nocap,nourl" >}}

{{< note >}}The first five characters of an instruction will suffice.{{< /note >}}

---

#### Additional examples

This example shows tile generation with titles in the center and titles in different styles.

{{< highlight css >}}
src="unknown01.jpg,unknown02.jpg,unknown03.jpg,unknown04.jpg,unknown05.jpg,unknown06.jpg"
caption="*Image 01*,~~Image 02~~,**Image 03**,*Image 04*,~~Image 05~~,**Image 06**"
cappos="middle"
capcol="white"
{{</ highlight>}}

{{< img src="unknown01.jpg,unknown02.jpg,unknown03.jpg,unknown04.jpg,unknown05.jpg,unknown06.jpg" caption="*Image 01*,~~Image 02~~,**Image 03**,*Image 04*,~~Image 05~~,**Image 06**" cappos="middle" capcol="white" >}}
