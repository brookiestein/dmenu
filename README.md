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

If you use dwm, can add this lines of code to your config.h:
```
static const char *dmenucmd[]                   = { "dmenu_run", "-l", "20", "-c", "-m", dmenumon, "-fn", dmenufont, "-nb", col_gray1,
                                                "-nf", col_gray3, "-sb", col_cyan, "-sf", col_gray4, NULL };
```

See the man page for more details.
