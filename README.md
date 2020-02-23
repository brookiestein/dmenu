**dmenu - dynamic menu**
====================
dmenu is an efficient dynamic menu for X.


**Requirements**
------------
In order to build dmenu you need the Xlib header files.


**Installation**
------------
Edit config.mk to match your local setup (dmenu is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu:

```
# for i in $(ls -1 patches/); do patch -i patches/$i; done
# make clean install
```

**Running dmenu**
-------------
Using the -c flag produce that dmenu start centered.
See the man page for more details.
