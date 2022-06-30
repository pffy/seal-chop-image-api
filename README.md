
# **SEALCHOP** is a simple seal chop image Web API. You can create Chinese or Korean seal chops.

### Quick Start

To get started, you can simply type the following URL into your browser:

```bash
https://png.sealchop.com/
```

You should see something similar to this:

<img width="200" src="https://png.sealchop.com/">

**This is the default seal chop image.** It appears when you type the base URL with no custom settings.

The dimensions of the PNG image are 1000 by 1000 pixels. All the preview images in this tutorial have been scaled down in size for your convenience.

Making your own chop is easy! You can make a custom chop by adding parameters to the base seal chop image URL.

### Chinese name chop

For example, you can change the Chinese name by simply setting the `x` parameter as follows:

```bash
https://png.sealchop.com/?x=貝聿銘
```

This will change the seal chop image into something similar to the image below:

<img width="200" src="https://png.sealchop.com/?x=貝聿銘">

### Korean name chop

You can also use Korean characters to create Korean seal chops.

For example, instead of entering a Chinese name, you can enter the following Korean name to change the image:

```bash
https://png.sealchop.com/?x=소정희
```

The image now becomes a Korean seal chop.

<img width="200" src="https://png.sealchop.com/?x=소정희">

At this time, you may enter 1, 2 or 3 characters for the Chinese or Korean seal chop name.

> **NOTE**: Many operating systems require the addition of language keyboards or input method editors to enter Chinese or Korean characters.

## Colors

### Paper Color

If you are viewing this documention in dark mode, you may have noticed that the four white corners of the seal chop image stand out against the black background. 

To allow the chop to better blend with its context, the `p` (paper) parameter can be changed as follows:

```bash
https://png.sealchop.com/?p=000000
```

The color `000000` is black, as defined by the hex triplet (6-digit hexadecimal).

Now, this image blends with the black background:

<img width="200" src="https://png.sealchop.com/?p=000000">


### Background Color

This is the most prominent color in the seal chop image.

```bash
https://png.sealchop.com/?b=FF6600
```

The image background section is now a shade of orange (`FF6600`) and looks similar to the image below:

<img width="200" src="https://png.sealchop.com/?b=FF6600">


### Foreground Color

This color provides a text area for the Chinese or Korean text.

You can change the foreground color using the `f` parameter:

```bash
https://png.sealchop.com/?f=FFFF00
```

The image foreground is now yellow (`FFFF00`) and looks similar to the image below:

<img width="200" src="https://png.sealchop.com/?f=FFFF00">



### Ink Color

This is the color of the Chinese or Korean text.

You can change the ink color using the `i` parameter:

```bash
https://png.sealchop.com/?i=0000FF
```

The image text is now blue (`0000FF`).

<img width="200" src="https://png.sealchop.com/?i=0000FF">

### Combining parameters

You can combine the parameters using the `&` (ampersand) between parameters

For example:

```bash
https://png.sealchop.com/?i=0000FF&f=00FF00&b=FF00FF
```

You will get a resultant image similar to this:

<img width="200" src="https://png.sealchop.com/?i=0000FF&f=00FF00&b=FF00FF">


## Version

This is **Version 8** of the seal chop image API.

## Synopsis

The following is a synopsis of the seal chop image API parameters:

`-` | data type | notes
:---: | :---: | :---
`x` | UTF-8 encoded Chinese or Korean character text | "xingming", the personal name. Non-Chinese or non-Korean characters are ignored
`p` | 6-digit hexadecimal color text (hex triplet) | "paper", the color below the chop. Only valid hex colors are accepted. All other input ignored.
`b` | 6-digit hexadecimal color text (hex triplet) | "background", the most prominent chop color. Only valid hex colors are accepted. All other input ignored.
`f` | 6-digit hexadecimal color text (hex triplet) | "foreground", the text area for the ink. Only valid hex colors are accepted. All other input ignored.
`i` | 6-digit hexadecimal color text (hex triplet) | "ink", the characters in the foreground. Only valid hex colors are accepted. All other input ignored.


