Elemenity Linux kernel
============

This repository contains the source code for the Linux
Kernel used on Elemenity devices.

https://www.elemenity.com/

Since most users are likely to be using x86 based computers,
we have included convenience scripts to cross-compile
the kernel. This allows you to use your (likely much faster)
x86 based computer to build the kernel for an aarch64 device.

## Building
```
make -f Makefile.elemenity config
# make your config changes
make -f Makefile.elemenity build
```

## Other documentation

There are several guides for kernel developers and users. These guides can
be rendered in a number of formats, like HTML and PDF. Please read
Documentation/admin-guide/README.rst first.

In order to build the documentation, use ``make htmldocs`` or
``make pdfdocs``.  The formatted documentation can also be read online at:

    https://www.kernel.org/doc/html/latest/

There are various text files in the Documentation/ subdirectory,
several of them using the Restructured Text markup notation.

Please read the Documentation/process/changes.rst file, as it contains the
requirements for building and running the kernel, and information about
the problems which may result by upgrading your kernel.
