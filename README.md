# Generic-Blitz-Slave
 
Quick and Dirty Readme.

To build this you require vasm68k_mot.
http://sun.hasenbraten.de/vasm/bin/rel/vasmm68k_mot_Win64.zip

and some include files from WHDLOAD dev.
and the Amiga NDK.
Which I have compiled into includes.zip since it is annoying to find them all

Then run the build.cmd file.

# To make it your own.
Atm it is setup to be an A1200 with 2Meg of Chip, running WB3.1, with AGA enabled, with the game able to be normally ran from HDD.
I will add slaves for 1.3, and running from a floppy disk soon.
If you have the whdload-dev package, look at the Generic Slaves found here.
http://www.whdload.de/whdload/GenericKick14.lha

Anyway, to modify it for your blitz program:
## Changes required
These lines specify how many kb of ram you want to allocate.

currently set to 2meg chip.

### Line 29:
CHIPMEMSIZE	= $1ff000	;size of chip memory

### Line 30:
FASTMEMSIZE	= $00000	;size of fast memory

### Lines 67 - 71:
These are the text which appear as the splash for WHDload.

### Line 160:
This is the Exe you want to load and run

Also Jotd, has alot of slaves on his github, if you like 68k asm haha.
https://github.com/jotd666/whdload_slaves
