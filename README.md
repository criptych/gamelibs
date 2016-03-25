# Game Development Libraries and Tools

A collection of useful libraries and tools for game development.  The [table]
below highlights each library with its (source and/or API) language and
license.  Following is a full library [listing] with brief descriptions and
links to downloads and documentation.

[table]: #summary
[listing]: #base-libraries

## About this list

The greater part of these libraries are free open-source (FOSS) with various
licenses including **zlib**, BSD, MIT, and GPL; a few have proprietary licenses
but are free to use; and at least one (actually a collection in its own right)
has been released into the public domain.

I began putting this together for my own use, to have a central repository of
useful libraries (similar to [AwesomeC++], among others) from which to choose
rather than continually hunting down each one “in the wild.”  I also added most
of the libraries as submodules in order to install/update the whole collection
with just a few commands:  `git submodule update --init` clones all submodules;
`git submodule foreach git pull` updates them to the latest upstream commit.

The libraries in this list were primarily selected for their usefulness in game
development, but many are applicable to other types of projects as well.

[AwesomeC++]: https://github.com/fffaraz/awesome-cpp

## Sources

The source links below reference (where possible) the official/primary source
repository for each project, many of which are on GitHub.  Additionally, if a
project has a mirror on GitHub (or elsewhere for projects whose primary source
is GitHub) – even an unofficial one, as long as it is kept reasonably
up-to-date – that is also listed.

## Corrections & Suggestions

If you notice an error in the list (wrong language, license, link) or think
something needs a new or different category, create an [issue] or pull request.
Likewise, if you know of a library that would fit well on this list – C/C++
API, useful in “multimedia” applications, preferably free and open-source – and
you don't see it here, create an [issue] and I'll check it out.  (I'd prefer
not to use pull requests for this.)

[issue]: http://github.com/criptych/gamelibs/issues/new

--------------------------------------------------------------------------------

## Summary

Group               | Library           | Language  |    |    |    | License
:-------------------|:------------------|:----------|:--:|:--:|:--:|:----------
**Base Libraries**  | [SDL2]            | C         |![C]|![P]|    | zlib
                    | [SFML]            | C++       |![C]|    |    | zlib
                    | [GLFW]            | C         |![C]|    |    | zlib
**Graphics**        | [OpenGL]          | C         |    |    |    | API only
                    | [GLAD]            | C/C++     |![C]|    |    | MIT
                    | [GLEW]            | C         |![C]|    |    | BSD
                    | [GLLoadGen]       | C/C++     |    |![P]|    | MIT
**Audio**           | [FMOD Studio]     | C++       |    |    |    | Prop.
                    | [OpenAL]          | C         |    |    |    | API only
                    | [OpenAL-Soft]     | C         |![C]|    |    | LGPL
                    | [Lyd]             | C         |    |    |![A]| ISC
**Physics**         | [Box2D]           | C++       |![C]|![P]|    | zlib
                    | [Bullet]          | C++       |![C]|![P]|    | zlib
                    | [Chipmunk2D]      | C         |![C]|    |    | MIT
**Math**            | [GLM]             | C++       |![C]|    |    | MIT
                    | [Graphene]        | C         |    |    |![A]| MIT
**Serialization**   | [Jansson]         | C         |![C]|    |    | MIT
                    | [MessagePack]     | C         |![C]|    |    | Boost
                    | [TinyXML2]        | C++       |![C]|    |    | zlib
                    | [YAML]            | C         |![C]|    |    | MIT
**Scripting**       | [Lua]             | C         |![C]|    |    | MIT
                    | [LuaJIT]          | C         |![C]|    |    | MIT
                    | [MoonScript]      | Lua       |    |    |![A]| MIT
                    | [Python]          | C         |    |    |![A]| PSF
                    | [Ruby]            | C         |    |    |![A]| BSD
                    | [mruby]           | C         |    |    |![R]| MIT
                    | [Squirrel]        | C++       |    |    |![A]| MIT
**Networking**      | [cURL]            | C         |![C]|    |    | MIT
                    | [ENet]            | C         |![C]|![P]|    | MIT
**AI**              | [FANN]            | C         |![C]|    |    | LGPL
                    | [MicroPather]     | C++       |    |    |![A]| zlib
**Miscellaneous**   | [Catch]           | C++       |    |    |    | Boost
                    | [Discount]        | C         |    |    |![A]| BSD
                    | [ImGui]           | C++       |    |    |    | MIT
                    | [Open Steamworks] | C++       |    |    |![M]| Other
                    | [PhysicsFS]       | C         |![C]|    |    | zlib
                    | [STB Nothings]    | C         |    |    |![M]| -
                    | [Steamworks]      | C++       |    |    |    | Prop.
**Tools**           | [CMake]           | C++       |![C]|    |    | BSD
                    | [Ninja]           | C++       |    |    |    | Apache
                    | [Premake]         | Lua       |    |![P]|![A]| BSD
                    | [SCons]           | Python    |    |    |![S]| MIT

[A]: <.image/make.png> "Build with Autoconf/Automake/Make"
[C]: <.image/cmake.png> "Build with CMake"
[M]: <.image/msvc.png> "Build with Visual Studio"
[P]: <.image/premake.png> "Build with Premake4"
[R]: <.image/rake.png> "Build with Rake"
[S]: <.image/scons.png> "Build with SCons"

[Box2D]: #box2d
[Bullet]: #bullet
[Catch]: #catch
[Chipmunk2D]: #chipmunk2d
[CMake]: #cmake
[cURL]: #curl
[Discount]: #discount
[ENet]: #enet
[FANN]: #fann
[FMOD Studio]: #fmod-studio
[GLAD]: #glad
[GLEW]: #glew
[GLFW]: #glfw
[GLLoadGen]: #glloadgen
[GLM]: #glm
[Graphene]: #graphene
[ImGui]: #imgui
[Jansson]: #jansson
[Lua]: #lua
[LuaJIT]: #luajit
[Lyd]: #lyd
[MessagePack]: #messagepack
[MicroPather]: #micropather
[MoonScript]: #moonscript
[mruby]: #mruby
[Ninja]: #ninja
[OpenAL]: #openal
[OpenAL-Soft]: #openal-soft
[OpenGL]: #opengl
[Open Steamworks]: #open-steamworks
[PhysicsFS]: #physicsfs
[Premake]: #premake
[Python]: #python
[Ruby]: #ruby
[SCons]: #scons
[SDL2]: #sdl2
[SFML]: #sfml
[Squirrel]: #squirrel
[STB Nothings]: #stb-nothings
[Steamworks]: #steamworks
[TinyXML2]: #tinyxml2
[YAML]: #yaml

--------------------------------------------------------------------------------

## Base Libraries

Input and event handling, windowing, graphics context handling, and sometimes
include other common services such as graphics, audio, and resource management.

### SDL2

2D graphics (software or hardware-accelerated); OpenGL support if requested;
basic audio playback; basic I/O support.  Additional features can be added
through a selection of support libraries.

- Website: <http://libsdl.org/>
- License: [zlib](http://www.libsdl.org/license.php)
- Source: [Website](http://hg.libsdl.org/SDL)
- Mirror: [GitHub](http://github.com/spurious/SDL-mirror)

### SFML

2D graphics (through OpenGL); buffered and streaming audio playback; support
for loading various image, font, and audio file formats.

- Website: <http://sfml-dev.org/>
- License: [zlib](http://www.sfml-dev.org/license.php)
- Source: [GitHub](https://github.com/SFML/SFML)

### GLFW

Lightweight base library that provides a minimum of extra features.

- Website: <http://www.glfw.org/>
- License: [zlib](http://www.glfw.org/license.html)
- Source: [GitHub](https://github.com/glfw/glfw)

--------------------------------------------------------------------------------

## Graphics

Render visuals to an on-screen or off-screen surface, including support
libraries for using such functionality.

### OpenGL

API for accelerated 2D and 3D graphics.

- Website: <https://www.opengl.org/>
- License: [None](https://www.sgi.com/tech/opengl/) (API only)
- Source: [Registry](https://cvs.khronos.org/svn/repos/ogl/trunk/doc/registry/public/api/)

### GLAD

Detects and enables OpenGL extensions in a client application.

- Website: <http://glad.dav1d.de/>
- License: [MIT](https://github.com/Dav1dde/glad/blob/master/LICENSE)
- Source: [GitHub](https://github.com/Dav1dde/glad)

### GLEW

Detects and enables OpenGL extensions in a client application.

- Website: <http://glew.sourceforge.net/>
- License: [BSD](http://glew.sourceforge.net/glew.txt)
- Source: [GitHub](https://github.com/nigels-com/glew)
- Mirror: [SourceForge](git://git.code.sf.net/p/glew/code)

### GLLoadGen

Detects and enables OpenGL extensions in a client application.

- Website: <https://bitbucket.org/alfonse/glloadgen/src>
- License: [MIT]()
- Source: [BitBucket](https://bitbucket.org/alfonse/glloadgen)

--------------------------------------------------------------------------------

## Audio

Render sound effects and music to an audio device, including support libraries
for using such functionality.

### FMOD Studio

API for high-level audio management and playback.

- Website: <http://www.fmod.org/>
- License: [Proprietary](http://www.fmod.org/files/public/LICENSE.TXT)
- Source: None

### OpenAL

API for advanced 3D audio.

- Website: <https://www.openal.org/>
- License: None? (API only)
- Source: None

### OpenAL-Soft

Free, open-source software implementation of OpenAL.

- Website: <http://openal-soft.org/>
- License: [LGPL](http://openal-soft.org/)
- Source: [GitHub](https://github.com/kcat/openal-soft)

### Lyd

Realtime audio-synthesis engine.

- Website: <http://pippin.gimp.org/lyd/>
- License: [ISC](http://pippin.gimp.org/lyd/)
- Source: [Website](http://pippin.gimp.org/git/lyd)
- Mirror: [GitHub](https://github.com/hodefoting/lyd)

--------------------------------------------------------------------------------

## Physics

Simulate 2D and 3D dynamic physics.  Usually geared toward performance over
precision, but may also be tunable.

### Box2D

2D physics engine.

- Website: <http://box2d.org/>
- License: [zlib](http://box2d.org/about/)
- Source: [GitHub](https://github.com/erincatto/Box2D)

### Bullet

3D physics engine.

- Website: <http://bulletphysics.org/>
- License: [zlib](https://github.com/bulletphysics/bullet3)
- Source: [GitHub](https://github.com/bulletphysics/bullet3)

### Chipmunk2D

2D physics engine.

- Website: <http://chipmunk-physics.net/>
- License: [MIT](https://github.com/slembcke/Chipmunk2D)
- Source: [GitHub](https://github.com/slembcke/Chipmunk2D)

--------------------------------------------------------------------------------

## Math

Provide extra mathematical functions above the standard library, especially
vector-matrix math (linear algebra) since it's useful for graphics.

### GLM

C++ library of vector and matrix math functions, designed to comply with GLSL
types and functions (but does not require OpenGL).

- Website: <http://glm.g-truc.net/>
- License: [MIT/“Happy Bunny”](http://glm.g-truc.net/copying.txt)
- Source: [GitHub](https://github.com/g-truc/glm)

### Graphene

C library of vector and matrix math functions.

- Website: <https://ebassi.github.io/graphene/>
- License: [MIT](https://ebassi.github.io/graphene/)
- Source: [GitHub](https://github.com/ebassi/graphene)

--------------------------------------------------------------------------------

## Serialization

Convert application data to and from a portable representation (usually text).

### Jansson

Library for JSON serialization.

- Website: <http://www.digip.org/jansson/>
- License: [MIT](http://www.digip.org/jansson/)
- Source: [GitHub](https://github.com/akheron/jansson)

### MessagePack

Library for compact binary object serialization.

- Website: <http://msgpack.org/>
- License: [Boost](https://github.com/msgpack/msgpack-c/blob/master/LICENSE_1_0.txt)
- Source: [GitHub](https://github.com/msgpack/msgpack-c)

### TinyXML2

Library for XML serialization.

- Website: <http://www.grinninglizard.com/tinyxml2/>
- License: [zlib](https://github.com/leethomason/tinyxml2)
- Source: [GitHub](https://github.com/leethomason/tinyxml2)

### yaml

Library for YAML serialization.

- Website: <http://www.yaml.org/>
- License: [MIT](https://github.com/yaml/libyaml)
- Source: [BitBucket](https://bitbucket.org/xi/libyaml)
- Mirror: [GitHub](https://github.com/yaml/libyaml)

--------------------------------------------------------------------------------

## Scripting

Enable scripting (by e.g. end users, non-programmers) to modify and extend a
program without recompiling, whether during testing to reduce development cycle
time, or after deployment to reduce the size of updates (often only a single
script needs to be updated, not the entire application).

### Lua

Simple but expressive high-level scripting language, designed for embedding.

- Website: <http://www.lua.org/>
- License: [MIT](http://www.lua.org/license.html)
- Source: [Website](http://www.lua.org/download.html)
- Mirror: [GitHub](https://github.com/LuaDist/lua)

### LuaJIT

Lua implementation with faster VM and JIT-compiler for even more performance.

- Website: <http://luajit.org/>
- License: [MIT](http://luajit.org/luajit.html)
- Source: [Website](http://luajit.org/git/luajit-2.0.git)
- Mirror: [GitHub](https://github.com/LuaDist/luajit)

### MoonScript

Ruby-like language that “compiles” to Lua.  (Requires Lua.)

- Website: <https://github.com/leafo/moonscript>
- License: [MIT](https://github.com/leafo/moonscript)
- Source: [GitHub](https://github.com/leafo/moonscript)

### Python

Powerful, widely-used scripting language with extensive library support.

- Website: <http://python.org/>
- License: [PSF](https://docs.python.org/3/license.html)
- Source: [Website](https://hg.python.org/cpython/)
- Mirror: [GitHub](https://github.com/python/cpython)

### Ruby

Concise yet powerful scripting language “with a focus on simplicity”.

- Website: <https://www.ruby-lang.org/>
- License: [BSD](https://www.ruby-lang.org/en/LICENSE.txt)
- Source: [GitHub](https://github.com/ruby/ruby)

### mruby

Embeddable standard-compliant version of Ruby.

- Website: <http://www.mruby.org/>
- License: [MIT](https://github.com/mruby/mruby/blob/master/MITL)
- Source: [GitHub](https://github.com/mruby/mruby)

### Squirrel

Sort of a mash-up of C++ and Lua.

- Website: <http://squirrel-lang.org/>
- License: [MIT](http://www.squirrel-lang.org/)
- Source: [SourceForge](http://sourceforge.net/projects/squirrel/)
- Mirror: [GitHub](https://github.com/pfalcon/squirrel-lang)

--------------------------------------------------------------------------------

## Networking

Send and receive data over the internet (or local network) for features like
DLC, UGC, and multiplayer.

### cURL

Library (and tool) for transparent access to internet resources.

- Website: <http://curl.haxx.se>
- License: [MIT](http://curl.haxx.se/docs/copyright.html)
- Source: [GitHub](https://github.com/bagder/curl)

### ENet

Reliable UDP network protocol.

- Website: <http://enet.bespin.org/>
- License: [MIT](http://enet.bespin.org/License.html)
- Source: [GitHub](https://github.com/lsalzman/enet)

--------------------------------------------------------------------------------

## Artificial Intelligence

Give enemies, NPCs, player units, etc. the ability to “think” for themselves.

### FANN

Fast Automatic Neural Networks, useful for developing and training AIs.

- Website: <http://leenissen.dk/fann/>
- License: [LGPL](http://leenissen.dk/fann/)
- Source: [GitHub](https://github.com/libfann/fann)

### MicroPather

Generic A* solver for pathfinding.

- Website: <http://www.grinninglizard.com/MicroPather/>
- License: [zlib](https://github.com/leethomason/MicroPather/blob/master/micropather.cpp)
- Source: [GitHub](https://github.com/leethomason/MicroPather)

--------------------------------------------------------------------------------

## Miscellaneous

### Catch

Header-only C++ unit test library.

- Website: <https://github.com/philsquared/Catch>
- License: [Boost](https://github.com/philsquared/Catch/blob/master/LICENSE_1_0.txt)
- Source: [GitHub](https://github.com/philsquared/Catch)

### Discount

Markdown parser with HTML renderer.

- Website: <http://www.pell.portland.or.us/~orc/Code/discount/>
- License: [BSD](http://www.pell.portland.or.us/~orc/Code/discount/COPYRIGHT.html)
- Source: [Website](http://www.pell.portland.or.us/~orc/Code/discount/discount-2.1.8a.tar.bz2)
- Mirror: [GitHub](http://github.com/Orc/discount)

### ImGui

Light-weight immediate mode GUI.

- Website: <http://www.patreon.com/imgui>
- License: [MIT](https://github.com/ocornut/imgui/blob/master/LICENSE)
- Source: [GitHub](https://github.com/ocornut/imgui)

### Open Steamworks

Reverse-engineered Steamworks API library.

- Website: <https://github.com/SteamRE/open-steamworks>
- License: Unknown
- Source: [GitHub](https://github.com/SteamRE/open-steamworks)

### PhysicsFS

Virtual filesystem with write-isolation.

- Website: <https://icculus.org/physfs/>
- License: zlib
- Source: [Website](http://hg.icculus.org/icculus/physfs/)

### STB

Collection of various helpful tools for loading images and fonts, generating
Perlin noise, and more.

- Website: <https://github.com/nothings/stb>
- License: [Public domain](https://github.com/nothings/stb)
- Source: [GitHub](https://github.com/nothings/stb)

### Steamworks

API for integration with Steam platform.

- Website: <https://partner.steamgames.com/>
- License: [Proprietary](https://partner.steamgames.com/documentation/sdk_access_agreement)
- Source: None

--------------------------------------------------------------------------------

## Tools

Useful development tools, especially build tools right now.

### CMake

Powerful build script generator.

- Website: <https://cmake.org/>
- License: [BSD](https://cmake.org/licensing/)
- Source: [Website](https://cmake.org/cmake.git)
- Mirror: [GitHub](https://github.com/Kitware/CMake)

### Ninja

Ultra-fast low-level build tool.

- Website: <https://ninja-build.org/>
- License: [Apache](https://github.com/ninja-build/ninja/blob/master/COPYING)
- Source: [GitHub](https://github.com/ninja-build/ninja)

### Premake

Build script generator based on Lua.  (Includes Lua.)

- Website: <https://premake.github.io/>
- License: [BSD](https://github.com/premake/premake-core/blob/master/LICENSE.txt)
- Source: [GitHub](https://github.com/premake/premake-core)

### SCons

Fully-integrated build system based on Python.  (Requires Python.)

- Website: <http://www.scons.org/>
- License: [MIT](https://bitbucket.org/scons/scons)
- Source: [BitBucket](https://bitbucket.org/scons/scons)

--------------------------------------------------------------------------------
