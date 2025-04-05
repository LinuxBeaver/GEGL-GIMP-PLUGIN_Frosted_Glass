# Frosted Glass

This GIMP Plugin makes a frosted glass effect with GEGL 

![image](https://github.com/user-attachments/assets/614fa2cd-2abe-44ef-b02a-a98cab3109b9)

![image](https://github.com/user-attachments/assets/28fa1a40-082a-45f8-8952-def4a4d26b16)



## Directory to put Binaries (They do NOT go in the normal plugins folder)

**Windows**

 `C:\Users\(USERNAME)\AppData\Local\gegl-0.4\plug-ins`

 **Linux**

`~/.local/share/gegl-0.4/plug-ins`

 **Linux (Flatpak includes Chromebook)**

`~/.var/app/org.gimp.GIMP/data/gegl-0.4/plug-ins`

Then Restart Gimp and go to Filters>Blur>Frosted Glass or just search for it with /


## Compiling and Installing

### Linux

To compile and install you will need the GEGL header files (`libgegl-dev` on
Debian based distributions or `gegl` on Arch Linux) and meson (`meson` on
most distributions).

```bash
meson setup --buildtype=release build
ninja -C build

```

### Windows

The easiest way to compile this project on Windows is by using msys2.  Download
and install it from here: https://www.msys2.org/

Open a msys2 terminal with `C:\msys64\mingw64.exe`.  Run the following to
install required build dependencies:

```bash
pacman --noconfirm -S base-devel mingw-w64-x86_64-toolchain mingw-w64-x86_64-meson mingw-w64-x86_64-gegl
```

Then build the same way you would on Linux:

```bash
meson setup --buildtype=release build
ninja -C build
```

## more previews of this based plugin

![image](https://github.com/user-attachments/assets/bdbd303d-da1b-4abd-86ff-13fc15540fe2)


