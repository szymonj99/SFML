# SFML switch port
This is a Switch port of the SFML libraries

## Dependencies
Before building, you must have devKitPro setup.

You only need libNX to build, but you need these libraries to link against:

  + OpenAL / [MojoAL](https://github.com/TomBebb/mojoAL-switch)
  + SDL2 (if using MojoAL)
  + LibNX
  + FLAC
  + Vorbis libraries
  + LibOGG
  + Mesa
  + LibPNG
  + ZLib
  + Nouveau DRM driver
  + GLAD
  + BZip2


## Building

1. Make build directory:

```bash
mkdir build
```

2. Run CMake to generate makefile:

```bash
cmake .. -DCMAKE_TOOLCHAIN_FILE=../cmake/toolchains/DevkitA64Libnx.cmake
```

3. Build binaries:

```bash
make -j 8
```

4. Static libraries were generated in the lib/ folder.

## Usage

I usually copy the .a libraries to $DEVKITPRO/portlibs/switch/lib after to simplify using the lib.


## Examples
Check out the examples [here](https://github.com/TomBebb/switch-examples/tree/master/sfml) for an example of how to set-up linking.




[![SFML logo](https://www.sfml-dev.org/images/logo.png)](https://www.sfml-dev.org)

# SFML — Simple and Fast Multimedia Library

SFML is a simple, fast, cross-platform and object-oriented multimedia API. It provides access to windowing, graphics, audio and network. It is written in C++, and has bindings for various languages such as C, .Net, Ruby, Python.

## State of Development

SFML is currently in an interesting state of development, which can quickly become confusing if you aren't following it closely. As such we want to clarify where to get which version.

-   The [`master`](https://github.com/SFML/SFML/tree/master) branch contains work in progress for the next major version SFML 3. As such it's considered unstable, but any testing and feedback is highly appreciated.
-   The [`2.6.x`](https://github.com/SFML/SFML/tree/2.6.x) branch is the nearly complete next minor version SFML 2.6, which should be very stable, even if it hasn't been officially released yet.
-   The [`2.5.1`](https://github.com/SFML/SFML/tree/2.5.1) tag is the last official SFML release, but it lacks a lot of fixes and features that can already be found on the `2.6.x` branch.

## Download

-   You can get the latest official release on [SFML's website](https://www.sfml-dev.org/download.php).
-   You can also get the source code of the current development version from the [Git repository](https://github.com/SFML/SFML).
-   Alternatively, you can get the latest snapshot / artifact builds from the [artifacts storage](https://artifacts.sfml-dev.org/by-branch/master/).

## Install

Follow the instructions of the [tutorials](https://www.sfml-dev.org/tutorials/), there is one for each platform/compiler that SFML supports.

## Learn

There are several places to learn SFML:

-   The [official tutorials](https://www.sfml-dev.org/tutorials/)
-   The [online API documentation](https://www.sfml-dev.org/documentation/)
-   The [community wiki](https://github.com/SFML/SFML/wiki/)

## Community

Here are some useful community links:

-   [Discord](https://discord.gg/nr4X7Fh)
-   [Twitter](https://twitter.com/sfmldev)
-   [Forum](https://en.sfml-dev.org/forums/) ([French](https://fr.sfml-dev.org/forums/))

## Contribute

SFML is an open-source project, and it needs your help to go on growing and improving. If you want to get involved and suggest some additional features, file a bug report or submit a patch, please have a look at the [contribution guidelines](https://www.sfml-dev.org/contribute.php).

## Authors

-   Laurent Gomila (laurent@sfml-dev.org)
-   Marco Antognini (hiura@sfml-dev.org)
-   binary1248 (binary1248@hotmail.com)
-   Lukas Dürrenberger (eXpl0it3r@sfml-dev.org)
-   Jonathan De Wachter (dewachter.jonathan@gmail.com)
-   Jan Haller (bromeon@sfml-dev.org)
-   Mario Liebisch (mario@sfml-dev.org)
-   Stefan Schindler (tank@sfml-dev.org)
-   Artur Moreira (artturmoreira@gmail.com)
-   Vittorio Romeo (vittorioromeo@sfml-dev.org)
-   And many other members of the SFML community

## License

The SFML libraries and source code are distributed under the [zlib/libpng license](https://opensource.org/licenses/Zlib). See [license.md](license.md). External libraries used by SFML are distributed under their own licenses.

In short, SFML is free for any use (commercial or personal, proprietary or open-source). You can use SFML in your project without any restriction. You can even omit to mention that you use SFML -- although it would be appreciated.

## External libraries used by SFML

-   [_OpenAL-Soft_](https://github.com/kcat/openal-soft) is under the [LGPL license](https://github.com/kcat/openal-soft/blob/master/COPYING)
-   [_stb_image_ and _stb_image_write_](https://github.com/nothings/stb) are [public domain](https://github.com/nothings/stb/blob/master/LICENSE)
-   [_freetype_](https://gitlab.freedesktop.org/freetype/freetype) is under the [FreeType license or the GPL license](https://gitlab.freedesktop.org/freetype/freetype/-/blob/master/LICENSE.TXT)
-   [_libogg_](https://gitlab.xiph.org/xiph/ogg) is under the [BSD license](https://gitlab.xiph.org/xiph/ogg/-/blob/master/COPYING)
-   [_libvorbis_](https://gitlab.xiph.org/xiph/vorbis) is under the [BSD license](https://gitlab.xiph.org/xiph/vorbis/-/blob/master/COPYING)
-   [_libflac_](https://gitlab.xiph.org/xiph/flac) is under the [BSD license](https://gitlab.xiph.org/xiph/flac/-/blob/master/COPYING.Xiph)
-   [_minimp3_](https://github.com/lieff/minimp3) is under the [CC0 license](https://github.com/lieff/minimp3/blob/master/LICENSE)
