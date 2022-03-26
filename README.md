# moba-terminal-script
Open `cygwin64` and `Msys2` terminal in MobaXterm.  

<image src="./readmes/screenshot.png" height=480>  

## How to use
Open MobaXterm and click `Session|Shell`, select `Cmd` and put this script in `Advanced Shell settings` tag. If you want use in unbuntu, please replace the `set` to `export`.  

## Script
* Open cygwin64 in windows:  
  ```bat
  set "HOME=/home/funte"
  "D:/dev/bins/cygwin64/bin/bash" --login
  ```
* Open default `msys2` in windows:  
  ```bat
  set MSYSTEM=MSYS
  set "MSYS2=c:/msys64"
  set "HOME=/home/funte"
  "%MSYS2%/usr/bin/bash" --login
  ```
* Open `Msys2-Mingw64` in windows:  
  ```bat
  set MSYSTEM=MINGW64
  set "MSYS2=c:/msys64"
  set "HOME=/home/funte"
  "%MSYS2%/usr/bin/bash" --login
  ```
* Other possible `MSYSTEM` values: `MINGW32, CLANG64, CLANGARM64, UCRT64`  
