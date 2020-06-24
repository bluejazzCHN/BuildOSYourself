# BuildOSYourself
Log the activities that study to build a simple OS.

## Enviroment
install and config steps that you can find from search.

+ [Bochs](http://bochs.sourceforge.net/) 

+ [Nasm](https://www.nasm.us/)

## First Step: Build boot

-- 1 write code in mbr.S
```
nasm mbr.S -o mbr.bin
```

-- 2 use nasm command to compile mbr.S to generate mbr.bin.

-- 3 use disk image creator (in the bochs installation folder) to generate boot.img.

-- 3 use dd command that you can find in C compiler fold write mbr.bin to boot.img.

-- 4 use bochs to config and boot vm from boot.img

-- 5 after boot, you will see "Start Boot" on VM screen.

