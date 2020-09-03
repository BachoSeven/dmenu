# Dmenu

Hi, I just applied a few patches from the suckless repository, feel free to use them!

### Applied Patches:
- Center
- Border (with command line option)
- fuzzymatch
- fuzzyhighlighting
- lineheight
- Xresources (compatible with fuzzy patches)
- Password support (-P)
- compatible with emoji support if you have [libxft-bgra](https://aur.archlinux.org/packages/libxft-bgra)

### More stuff
- paste binding is more intuitive (ctrl+v)

## Original README:

```
dmenu - dynamic menu
====================
dmenu is an efficient dynamic menu for X.


Requirements
------------
In order to build dmenu you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (dmenu is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu
(if necessary as root):

    make clean install


Running dmenu
-------------
See the man page for details.
```
