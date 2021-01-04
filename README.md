# msysCORE Extended

**msysCORE** consists of the [MSYS](http://www.mingw.org/wiki/MSYS) runtime plus
the basic support files for a standard [MSYS](http://www.mingw.org/wiki/MSYS)
installation. This project is part of the legacy [MinGW.org](http://mingw.org/)
project.

This repository contains the unofficial **msysCORE 1.0.19-2** release which
implement only one change, comparing to the official [msysCORE 1.0.19-1](https://sourceforge.net/projects/mingw/files/MSYS/Base/msys-core/msys-1.0.19-1/)
release: It's now possible to disable the [POSIX path conversion](http://mingw.org/wiki/Posix_path_conversion)
by setting the `MSYS_NO_PATHCONV` environment variable. This behaviour was
extracted from [Git for Windows](https://github.com/git-for-windows).

## Installation

1. Download the `msysCORE-1.0.19-2-msys-1.0.19-bin.tar.xz`.
2. Extract the `msys-1.0.dll` file from this package and move this file in your
   `%MSYSROOT%\msys\1.0\bin` directory, where `%MSYSROOT%` is the **MinGW** 
   installation directory (typically `C:\MinGW`).

## Compile

If you want to recompile this source, you will need to have a working 
[MSYS Toolchain](http://www.mingw.org/wiki/HOWTO_Create_an_MSYS_Build_Environment).

Then, follow the instructions in the `src/msysCORE.RELEASE_NOTES.txt` file.

## Links

* [How to stop MinGW and MSYS from mangling path names given at the command line](https://stackoverflow.com/a/34386471/3726096)
* [path-conversion: Prevent conversion of commandline flags.](https://github.com/git-for-windows/msys2-runtime/pull/11)
