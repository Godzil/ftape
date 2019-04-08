FTAPE
=====

This repository contain the sources of ftape 3.04d taken from Michael Bäuerle patch-set for kernel 2.6.36 ( http://micha.freeshell.org/qic117/QIC-117_patch.html ) to make it as an out of tree kernel module
and try to port it to more recent version of the kernel.

This repository currently only contain extracted files from Michael's patch file, out of tree compilable module will come later.


Background
----------

Because it was unmaintained, ftape was removed since kernel 2.6.20. But there are still people who use it for QIC-117 tapes (aka floppy tapes) or want to use it ... myself for example ;-)


Warnings
--------

Formatting of cartridges do not work.
It is no longer possible to have both floppy.ko and ftape.ko/zftape.ko loaded at the same time if the drives are connected to the same controller. Therefore none of them can be compiled into the kernel directly in this case if both drives should be usable.
Maybe this driver have problems on SMP machines.
Maybe this driver have problems on 64Bit x86 machines.
This patch was tested and work for me but there is no warranty! 