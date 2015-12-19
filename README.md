![MiltonLogo](http://i.imgur.com/hXxloIS.png)

Milton is a modern paint app.

### [Latest release (2015-09-25) pre-alpha](https://github.com/serge-rgb/milton/releases/tag/prealpha002)

![alpaca](http://i.imgur.com/k7E8k7r.png)

![alpaca](http://i.imgur.com/fJJZ0Bj.png)

![alpacaGif](http://i.imgur.com/QR8TPDJ.gif)

The Pitch
---------

One problem with digital art tools is that pixels are too constraining. It is liberating to not have to pick a resolution when starting something new, and to be able to export it to any size. Milton wants to provide that freedom.

Milton is open source, and runs on almost any machine. It has an efficient software renderer. It runs well on 10-year old laptops and on supercomputers. It is opinionated. There is no save button because this isn't the 80s anymore. Your work is persistent, with unlimited undo.

It is handmade, data oriented, gamma-correct, and user friendly.

Features
--------

- Infinite canvas

    ![zoooom](http://i.imgur.com/fqOhPlr.gif)

    You don't pick a resolution, and you don't work with pixels.  Your work is
    stored as a sequence of commands, and rendered on the fly. Once it's
    implemented, you will be able to export your work to bitmaps of arbitrary
    size.

- Simple

    Milton solves a single problem: draw without pixels. It doesn't pretend to be
    something more than that. The UI will be simple, with a "no-manual-needed" motto.

- Persistent

    No save button. Ctrl-S is *so* 1980's

- Wacom support

    Milton currently works with a Wacom intuos pen&touch on Windows and Linux (X11).
    OSX support is coming.

- Gamma-correct alpha blending and 32-bit floating point per channel

- Software rendered.

- Fast and light-weight

- Multi-platform

    Windows, Linux, OSX

- Open Source

    Milton is licensed under the GPL


What Milton is not:
-------------------

Milton is not an image editor or a vector graphics editor. It's a program that
lets you draw, sketch and paint.

User Manual
===========

While we get the GUI situation figured out, you can use the keyboard.

Keyboard Shortcuts
------------------

| Input                  | Action                |
| :--------------------: | --------------------: |
| `Space + Mouse Drag`   | Drag Canvas           |
| `0 - 9`                | Change brush opacity  |
| `[`                    | Make brush smaller    |
| `]`                    | Make brush larger     |
| `ctrl + z`             | Undo                  |
| `ctrl + y`             | Redo                  |
| `ctrl + backspace`     | Clear (not undoable!) |

Your work is kept in a file called MiltonPersist.mlt
Support for multiple files is coming. But right now you can just pan the canvas

How to Compile
==============

Milton targets Windows, Linux and OSX. 64 bit is recommended but not necessary.

Developed on:

* Windows 10 (Intel x64, NVidia GTX770)
* Linux Mint 17.03 (same machine)
* OSX 10.11 El Capitan (Macbook Pro mid 2012)

Also known to work on:

* Arch Linux on a laptop with Intel integrated graphics

Windows
-------

Requirements:

- CMake (for SDL)
- Visual Studio 2015 (Community Edition is fine.)

0. Open a developer console. You have at least two options:
    - Open "Visual Studio Command Prompt" and go to Milton's directory.
    - Use cmd.exe and run `scripts\vcvars.bat` to have the Visual Studio 2015 suite in your PATH. It will try to use the 64-bit version
1. Run `setup.bat` to build SDL
2. `build.bat`
3. Milton is compiled to `build\Milton.exe`

Linux
-----

Requirements:

- SDL2 development libraries. On Ubuntu, this is `apt-get install libsdl2-dev`
- The clang compiler.

Just run `make`

OSX
---

Requirements:

- CMake (for building SDL)

1. `./setup_osx.sh` to download dependencies and build SDL
2. `./build_osx.sh`
3. Milton is compiled to `./build/milton`

Roadmap
-------

See TODO.txt

Thank You
=========

* Inspiration / Education
    * Casey Muratori. This program would be very different (and much slower) if not for Handmade Hero

* Art
    * Milton's logo by the very talented [Perla Fierro](http://portafolio.eclat-studio.com/)

* Code
    * [Apoorva Joshi](http://apoorvaj.io) - Author of [Papaya](https://github.com/ApoorvaJ/Papaya) for joining forces and creating [EasyTab](https://github.com/ApoorvaJ/EasyTab).
    * [Michael Freundorfer](https://github.com/mordecai154)
    * [Joshua Mendoza](https://github.com/jomendoz)

* Rubber-ducking / Whiteboarding
    * Rodrigo Gonzalez del Cueto [@rdelcueto](https://twitter.com/rdelcueto)
    * Luis Eduardo Pérez
    * Mom

* The "Jueves Sensual" team :)
    * Axel Becerril
    * Ruben Bañuelos
    * Caro Barberena
    * Carlos Chilazo
    * Roberto Lapuente
    * Joshua Mendoza
    * Maximiliano Monterrubio
    * Santiago Montesinos
    * Aarón Reyes García
    * Vane Ugalde

