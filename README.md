#Clasqm's libraries for yab

## About my libraries

The following are libraries I have written:

### libclasqm_main: 
a variety of yab routines

### Routines: 
**WhereAmI$()**: returns the current directory from which the program is running

**OldWhereAmI$()**: works with older versions of yab, or use as fallback

**HPKGStatus()**: report app's status in the Haiku packaging system

**FileExists(fullpathname$)**: test if a file exists

**RandInt()**: returns a random integer between 0 and 32767

**RandInt0To9()**: returns a random integer between 0 and 9, inclusive

**StripLFoffSysCmd$()**: remove LF from the results of a system call

**TempDir$()**: returns the location of Haiku's TMP directory

**FileorDir()**: tests whether a passed pathname is a file or a directory

**FileorLink()**: tests whether a passed pathname is a file/directory or a symlink

**GetDimensions**: find the x or y dimensions of a window

**WorkspaceCurrent$**: find the current workspace

**WorkspaceTotal$**: find the total number of workspaces on a system

**WorkspaceSwitch, WorkspaceSwitch$**: switch to a specific workspace

### libclasqm_compat: 
Routines that mimic features or variations found in other forms of BASIC

These libraries are linked to */boot/home/config/settings/yab* by the packaging system.

## About the other libraries

These are just some yabasic libraries I have found scattered across the web. Some of them might still be useful for yab CLI application programming. I have bundled them here before they disappear. But please note that I don't  claim to have tested them or adapted them to yab. When I invent MoreTime(tm) I may do so, but for now they are just there for my fellow yab developers to play with.

I have not edited these libraries, just renamed some of them to give a more uniform structure to the collection (basically, starting them all with "libclasqm_"). The original filenames can be found within some files' comments. These libraries are NOT linked to* /boot/home/config/settings/yab* by default. Supplementary files are stored in the *lib/libclasqm* directory.

Copyright remains with the original authors, if anyone can still trace them after all this time. The fact that they were published as source code back before we all became obsessed with licences is taken as indicating that Public Domain licensing was intended. f any library or routine presented here is yours and you object to its inclusion, please inform me and I will remove it from the bundle.

Some of these libraries seem to have been written under earlier versions of yabasic, and need fixing. I have not tried to do this, on the basis that these will serve more as examples and inspiration, and besides, it depends on what exactly you want to use them for.

Most have built in documentation. To see it, type:

*yab -doc libclasqm_whatever*

**libclasqm_libini** - create and maintain .ini files.

**libclasqm_libcgi** - CGI handling routines

**libclasqm_dbf** - OK, technically this is not a library, though it would be trivial to convert it to one. It reads DBase III files, if anyone remembers those. A sample file is included.

**libstrings** - additional string-handling routines

**libclasqm_libgraph** - graphics routines for the Terminal

**libclasqm_libgui** - contains routines to add buttons to a Terminal interface. If you want to use these, you'll have to rename some of the routines (eg "button") as they clash with yab's own extensions to yabasic. It contains 2 fonts - these are NOT the .ybm files included - they are self-contained in DATA statements

**libclasqm_libimage** - routines to handle .pcx and .bmp files. Needs fixing: the COLOR command seems to have changed since it was written.

**libclasqm_scalfont** - a demonstration of using scalable fonts in the Terminal. Requires the 4 .ybm files (included).

**libclasqm_libtextgui** - routines for a text-based "GUI"

**libclasqm_libdeck** - routines to display playing cards in Terminal mode

**libclasqm_libdeck2** - routines to manipulate playing cards - requires libclasqm_libdeck

**libclasqm_libbits** - miscelaneous routines

## About the utilities##

The following CLI utlities are included in this HPKG:

**ShowDateInYabFormat**

**ShowDeskbarExpanded**

**ShowDeskbarHeight**

**ShowDeskbarPosition**

**ShowDeskbarWidth**

**ShowDeskbarX**

**ShowDeskbarY**

**ShowDesktopHeight**

**ShowDesktopWidth**

**ShowScrollbarWidth**

**ShowTabHeight**

Get it here: https://github.com/clasqm/libclasqm

Binaries: https://sourceforge.net/p/libclasqm/

 
