# LZWolf

LZWolf is a fork of Blzut3's ECWolf project. It still combines the original Wolfenstein 3D engine with the user experience of ZDoom to create the most user and mod author friendly Wolf3D source port.

Like ZDoom, LZWolf aims to support all games which use the Wolfenstein 3D engine including Blake Stone (coming in ECWolf 3.0), Corridor 7, Operation Body Count, Rise of the Triad, and Super 3D Noah's Ark.  LZWolf will also support Macintosh Wolfenstein 3D along with all of its user created missions (coming in ECWolf 2.0).

* Single binary runs all supported games.  (Wolfenstein 3D, Spear of Destiny, Super Noah's Ark 3D, ...)
* Full support for high resolution modes with aspect ratio correction.
* Modern control schemes (WASD + mouse + controller).
* Mac Wolf/S3DNA/ROTT style automap.
* Unlimited save slots.
* This is actually based on the Wolf3D engine instead of a recreation or forcing into a more modern engine.
    * Software rendered using the same 8-bit ray casting.
    
## PortMaster Changes

PM-LZWolf stays true to the original source with exception to the available resolutions. Since PortMaster is generally used with small-arm handhelds, with lower cpu and memory power, the ultra widescreen resolutions are not necessary. In addition, some custom resolutions
were missing. These can all be viewed and modified at the [sdlvideo.cpp](https://github.com/JeodC/pm-lzwolf/blob/main/src/sdlvideo.cpp#L383) file.

## Custom Features

LZWolf supports features not necessarily present in the official ECWolf project. The implementation may differ from ZDoom and the official ECWolf. Mods which are built on LZWolf should not be expected to work the same way on ECWolf!

* Parallax sky
* Damage types
* Halo lights (experimental)

## Mod Authoring

* Create mods without working with the source code!
    * Mods work with all supported platforms including Windows, Mac OS X, and Linux.
* Arbitrary high resolution texture, flat, and sprite support.
* Unlimited simultaneous moving pushwalls.
* Unlimited things.
* Unrestricted map size. (Although technical limits restrict GAMEMAPS format to 181x181.)
* Uses scripting formats and data formats similar to those of ZDoom.
    * Doom editing utilities work with ECWolf. (Except for levels)
    
## Compiling
```
git clone https://github.com/JeodC/pm-lzwolf
cd pm-lzwolf
mkdir build && cd build
cmake ..
make
strip lzwolf
```

Retrieve binaries `lzwolf` and `lzwolf.pk3`.

## Mod Compatibility

* Backwards compatibility for mods will not necessarily be kept.
* LZWolf does not gaurentee compatibility with ECWolf mods.

## LZWolf Links

* [Parent LZWolf](https://bitbucket.org/linuxwolf6/lzwolf)
* [Wiki](https://bitbucket.org/linuxwolf6/lzwolf/wiki)

## ECWolf Links

* [Website](http://maniacsvault.net/ecwolf/)
* [Forums](http://forum.drdteam.org/viewforum.php?f=174)
* [Wiki](http://maniacsvault.net/ecwolf/wiki/)
