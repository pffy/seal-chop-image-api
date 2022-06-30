
# **SEALCHOP** is a simple seal chop image Web API. You can create Chinese or Korean seal chops.

### Quick Start

To get started, you can simply type the following URL into your browser:

```bash
https://png.sealchop.com/
```

You should see something similar to this:

<img width="200" src="https://png.sealchop.com/">

**This is the default seal chop image.** It appears when you type the base URL with no custom settings.

The dimensions of the image are 1000 by 1000 pixels. The images in this tutorial have been scaled down for your convenience.

You can make a custom chop by adding parameters to the base seal chop image URL.

For example, you can change the Chinese name by simply setting the `x` parameter as follows:

```bash
https://png.sealchop.com/?x=貝聿銘
```

This will change the seal chop image into something similar to the image below:

<img width="200" src="https://png.sealchop.com/?x=貝聿銘">

You can also use Korean characters. 

For example, you can enter the following Korean name to change the image:

```bash
https://png.sealchop.com/?x=소정희
```

The image becomes a Korean seal chop.

<img width="200" src="https://png.sealchop.com/?x=소정희">

At this time, you may enter 1, 2 or 3 characters for the Chinese or Korean seal chop name.

> **NOTE**: Many operating systems require the addition of language keyboards or input method editors to enter Chinese or Korean characters.

## Synopsis

The following is a synopsis of seal chop image API parameters:

`-` | data type | notes
:---: | :---: | :---
`x` | UTF-8 encoded Chinese or Korean character text | "xingming", the personal name. Non-Chinese or non-Korean characters are ignored
`p` | 6-digit hexadecimal color text (hex triplet) | "paper", the color below the chop. Only valid hex colors are accepted. All other input ignored.
`b` | 6-digit hexadecimal color text (hex triplet) | "background", the most prominent chop color. Only valid hex colors are accepted. All other input ignored.
`f` | 6-digit hexadecimal color text (hex triplet) | "foreground", the text area for the ink. Only valid hex colors are accepted. All other input ignored.
`i` | 6-digit hexadecimal color text (hex triplet) | "ink", the characters in the foreground. Only valid hex colors are accepted. All other input ignored.

