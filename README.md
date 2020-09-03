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
- Mouse Buttons supported
- -r option to reject non-matching input

### More stuff
- paste binding is more intuitive (ctrl+v)
- compatible with emoji support if you have [libxft-bgra](https://aur.archlinux.org/packages/libxft-bgra)
- I (more or less regularly) merge new commits from `suckless` upstream and fix the applied patches; current version is `5.0`.

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
