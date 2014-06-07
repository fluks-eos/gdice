Description
===========

A GTK+ 3 dice with various different dices.

Requirements
============

Building the program requires GTK+ 3 and gstreamer-1.0 libraries.

Install
=======

 make [PREFIX=ABSOLUTE_PATH]
 make install

Notice, that you can't run the program after make, because the resources
are not yet copied to the paths in generated config.h.

Uninstall
=========

 make uninstall

Running make creates src/prefix file, containg $PREFIX, uninstall goal needs
that.

Screenshot
==========

![gdice](https://github.com/fluks/gdice/raw/master/gdice.png)
