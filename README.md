# Awesome micro:bit [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![micro:bit logo](https://i.imgur.com/rYLbkBh.jpg)](https://www.microbit.org)

A curated list of resources for the BBC micro:bit, a tiny programmable computer designed to make learning and teaching easy and fun! 
This embedded board has a Bluetooth capable microcontroller, USB interface, accelerometer, magnetometer, light and temperature sensors, 5x5 LED matrix, buttons, and accessible GPIO.

Inspired by the [Awesome lists](https://github.com/sindresorhus/awesome).

Contributions are welcome!

## Contents

- [Programming](#programming)
	- [Visual](#visual)
	- [Python](#python)
	- [JavaScript / MakeCode](#javascript-and-makecode)
	- [C/C++](#cc)
	- [Other micro:bit Languages](#other-microbit-languages)
	- [Other Interaction Languages](#other-interaction-languages)
- [Programming Tools](#programming-tools)
- [Mobile Apps](#mobile-apps)
- [ChromeOS Apps](#chromeos-apps)
- [Interface Chip](#interface-chip)
- [Hardware](#hardware)
- [CAD & 3D Printing](#cad--3d-printing)
- [Projects](#projects)
- [Articles](#articles)
- [Videos](#videos)
- [Books](#books)
- [Teaching Resources](#teaching-resources)
- [Community](#community)
- [Miscellaneous](#miscellaneous)


## Programming

### Visual

- [MakeCode](https://makecode.microbit.org) - Provides an in-browser emulator and a Blocks interface that generates JavaScript (TypeScript) code (Previously known as PXT).
- [Microsoft Blocks](https://www.microbit.co.uk/app/#create:xczaux) - Block interface that produces Touch Develop code. No longer in development and it's recommended to use MakeCode instead.
- [Code Kingdoms](https://www.microbit.co.uk/app/#create:tomwku) - Graphical interface that provides a transitioning experience from 'drag and drop' to text-based programming (JavaScript).
- [Scratch for BBC micro:bit](http://www.picaxe.com/BBC-microbit) - Using micro:bit with Scratch / S2Bot as a Bluetooth 'games controller' (needs specific BLED112 Bluetooth dongle).
- [Open Roberta Lab](http://lab.open-roberta.org) - Block programming environment design for programming robots, it also supports the micro:bit by generating MicroPython.
- [ScratchX micro:bit extension](https://llk.github.io/microbit-extension/) - Lets you control your micro:bit wirelessly using Scratch programming blocks.

### Python

- [MicroPython](http://microbit-micropython.readthedocs.io) - Port of MicroPython, a Python 3 implementation for microcontrollers and constrained environments.

##### MicroPython Editors

- [microbit.org Python editor](https://python.microbit.org) - The official online Python editor from the micro:bit foundation website.
- [microbit.co.uk Python editor](http://microbit.co.uk/app/#create:xyelfe) - Original Python editor from microbit.co.uk, contains an older version of MicroPython.
- [Mu](http://codewith.mu) - "Micro" editor for MicroPython and the BBC micro:bit.
- [create.withcode.uk](https://create.withcode.uk) - Python online editor and simulator that supports the micro:bit MicroPython ([instructions](http://community.computingatschool.org.uk/resources/4479)).
- [Atom microbit-micropython](https://github.com/wendlers/atom-microbit-micropython) - BBC micro:bit MicroPython support package for the Atom editor.
- [Thonny micro:bit](https://bitbucket.org/KauriRaba/thonny-microbit/wiki/installation-guide) - Plug-in for [Thonny](http://thonny.org), a Python IDE for beginners.
- [JetBrains IDEA/PyCharm IDE plugin](https://plugins.jetbrains.com/plugin/9777-micropython-support) - Support for MicroPython devices in IntelliJ IDEA and PyCharm.

##### MicroPython Libraries

- [Servo](https://github.com/microbit-playground/microbit-servo-class) - Simple class for controlling servos on the micro:bit via PWM.
- [PCA9685](https://github.com/gingemonster/PCA9685-Python-Microbit) - Simple class for using the PCA9685 16-Channel 12-bit PWM/Servo Driver via I2C.
- [MAX7219 7-segment](https://github.com/microbit-playground/matrix7seg) - MicroPython module for using a 7-segment display driven by a MAX7219 chip via SPI.
- [MAX7219 matrix](https://github.com/titimoby/microbit4all/blob/master/libraries/matrix7219.py) - MicroPython module for using a 8x8 Leds Matrix driven by a MAX7219 chip via SPI.
- [SSD1306](https://github.com/fizban99/microbit_ssd1306) - MicroPython library to control the OLED SSD1306 128x64 I2C with a micro:bit.
- [SSD1306 7seg](https://github.com/fizban99/microbit_ssd1306_7seg) - MicroPython library to use an SSD1306 OLED display as a 7 segment display.
- [SSD1306 SPI](https://github.com/fizban99/microbit_ssd1306spi) - MicroPython library to control the OLED SSD1306 128x64 display with a micro:bit via SPI.
- [HT16K33](https://bitbucket.org/thesheep/microbit-ht16k33) - MicroPython library for the HT16K33 LED matrix driver in multiple configurations (16x8, 8x8 or 8x8x2).
- [HC-SR04](https://github.com/fizban99/microbit_hcsr04) - Basic MicroPython library to read the distance from a HC-SR04 ultrasonic sensor using the SPI peripheral.
- [US-100](https://github.com/fizban99/microbit_us100) - Basic MicroPython library to read the distance from a US-100 ultrasonic sensor via UART.
- [KY038](https://github.com/fizban99/microbit_ky038) - MicroPython library to calibrate and use a sound sensor KY038, including clap counter functionality.
- [Nokia 5110 PCD8544 LCD](https://github.com/matneee/microbit-nokia5110-PCD8544-lcd) - Fast Micro:bit MicroPython controller for Nokia 5110 LCDs.
- [MPL115A1](https://github.com/hackscribble/microbit-MPL115A1-barometer) - MicroPython class to read the pressure and temperature readings from the NXP MPL115A1 SPI sensor.
- [24LCxxx EEPROM](https://github.com/matneee/microbit-I2C-EEPROM-24LCxxx-Read-Write) - Example Micro:bit functions to read and write to a Microchip I2C EEPROM.
- [ULN2003](https://github.com/IDWizard/uln2003) - Micropython code to drive stepper motors via ULN2003 darlington transistors.

##### Python Libraries

- [MicroPeri](https://github.com/c0d3st0rm/microperi) - Run Python programs on your computer with the same micro:bit MicroPython API and connecting a micro:bit as an external peripheral device or sensor.
- [microbit_stub](https://github.com/casnortheast/microbit_stub) - Python package that emulates the micro:bit as defined by the micro:bit MicroPython API.
- [bluezero](https://github.com/ukBaz/python-bluezero) - Python package to interface with Bluetooth devices, with examples for the micro:bit.
- [bitio](https://github.com/whaleygeek/bitio) - BBC micro:bit I/O library for Python. It allows you to run code in Python on a PC/Mac/Linux/Raspberry Pi and interact directly with the micro:bit.

##### Python Programming Tools

- [uFlash](https://github.com/ntoll/uflash/) - Utility for flashing the micro:bit with Python scripts and the MicroPython runtime.
- [MicroFs](https://github.com/ntoll/microfs) - Simple command line tool and module for interacting with the limited file system provided by MicroPython on the micro:bit.
- [Jupyter kernel for the micro:bit](https://github.com/takluyver/ubit_kernel) - Package that allows Jupyter interfaces to run MicroPython code directly on the micro:bit.

### JavaScript and MakeCode

- [MakeCode](https://makecode.microbit.org) - The Programming eXperience Toolkit for the micro:bit provides an in-browser emulator, a Blocks interface, and JavaScript (TypeScript) editor.
- [Espruino JavaScript](http://www.espruino.com/MicroBit) - JavaScript interpreter for microcontrollers. It also offers a WebIDE for written code and blocks.
- [Code Kingdoms](https://www.microbit.co.uk/app/#create:tomwku) - Graphical interface that provides a transitioning experience from 'drag and drop' to text-based programming (JavaScript).

##### MakeCode Libraries

- [Neopixel](https://github.com/Microsoft/pxt-neopixel) - Neo-Pixel package for pxt-microbit.
- [Filesystem](https://github.com/Microsoft/pxt-filesystem) - BETA package to support file system.
- [MAX6675](https://github.com/Microsoft/pxt-max6675) - Package for the MAX6675 component in PXT.
- [Bluetooth MAX6675](https://github.com/Microsoft/pxt-bluetooth-max6675) - Bluetooth service for the MAX6675 temperature probe.
- [Sonar](https://github.com/Microsoft/pxt-sonar) - Microsoft MakeCode package to handle sonar sensors and pings.
- [Bluetooth Temperature Sensor](https://github.com/Microsoft/pxt-bluetooth-temperature-sensor) - Bluetooth service to expose a temperature reading.
- [MIDI](https://github.com/Microsoft/pxt-midi) - MIDI interface for MakeCode - beta.
- [Bluetooth MIDI](https://github.com/Microsoft/pxt-bluetooth-midi) - Bluetooth Midi package for Microsoft Make Code - beta.
- [BlueDot](https://github.com/Microsoft/pxt-bluedot) - PXT package to support the BlueDot app - beta.
- [GY521](https://github.com/PaulDFoster/pxt-microbit-GY521) - PXT package for the Microbit to drive a MPU-6050 (GY-521).
- [UCL Junkrobot](https://github.com/chevyng/pxt-ucl-junkrobot) - Junk robot controlled using 28BYJ-48 stepper motors and HC-SR04 ultrasonic sensor.
- [BitBot](https://github.com/srs/pxt-bitbot) - BitBot Package for Microsoft PXT.
- [gamer:bit](https://github.com/sparkfun/pxt-gamer-bit) - SparkFun gamer:bit package for Microsoft MakeCode.
- [moto:bit](https://github.com/sparkfun/pxt-moto-bit) - MakeCode package for the SparkFun weather:bit board.
- [weather:bit](https://github.com/sparkfun/pxt-weather-bit) - Package to add support for the weather:bit add-on board from SparkFun.
- [SSD1306](https://github.com/Tinkertanker/pxt-ssd1306-microbit) - Package for SSD1306 OLED controller, based on the Adafruit Arduino library.
- [mi:node](https://github.com/minodekit/pxt-minode) - Mi:node kit(micro:bit IoT Starter Kit by element14) driver package for PXT/microbit.
- [Kitronik Servo Lite](https://github.com/KitronikLtd/pxt-kitronik-servo-lite) - Blocks that support Kitronik Servo:Lite board for the micro:bit.
- [Kitronik I2C 16 Servo](https://github.com/KitronikLtd/pxt-kitronik-I2C-16-servo) - Blocks for driving the Kitronik I2C 16 servo expansion board.
- [Kitronik motor driver](https://github.com/KitronikLtd/pxt-kitronik-motor-driver) - Blocks for driving the Kitronik micro:bit motor driver board.
- [Lego Power Functions](https://github.com/philipphenkel/pxt-powerfunctions) - Control your LEGO® Power Functions motors using your micro:bit with an infrared LED.
- [KY-040](https://github.com/Tinkertanker/pxt-ky040-microbit) - Tinkertanker package for the KY-040 rotary encoder.
- [Invent robot](https://github.com/techcampuk/pxt-invent) - This library provides a Microsoft PXT package for Invent robot.
- [Robotbit](https://github.com/KittenBot/pxt-robotbit) - Package for KittenBot Robotbit.
- [ubirch NB-IoT](https://github.com/ubirch/pxt-ubirch) - Package for sending signed data messages to the ubirch backend.
- [CCS811](https://github.com/ADataDate/pxt-airQuality) - Makecode Package for the CCS811 Air Quality Sensor.
- [DS1307](https://github.com/Tinkertanker/pxt-ds1307-microbit) - Tinkercademy MakeCode package for using the DS1307 real-time clock (beta).
- [HT16K33](https://github.com/Tinkertanker/pxt-ht16k33-alnum4) - Tinkercademy MakeCode Package for the HT16K33 I2C Alphanumeric Display (beta).
- [HoneyBit](https://github.com/HoneycombKits/pxt-HoneyBit) - A Honeycomb kits package for micro:bit MakeCode.

##### Node.js Libraries

- [node-bbc-microbit](https://github.com/sandeepmistry/node-bbc-microbit) - Control a micro:bit from Node.js using BLE.
- [node-bbc-microbit-io](https://github.com/sandeepmistry/node-bbc-microbit-io) - Johnny-Five (JavaScript Robotics and IoT programming framework) micro:bit IO Plugin.

##### JavaScript Browser Libraries

- [microBit.js](https://github.com/antefact/microBit.js) - JavaScript library to interact with BBC micro:bit using web bluetooth API.

##### JavaScript Programming Tools

- [PXT Command Line Tool](https://makecode.com/cli) - Use the command line to program the micro:bit with MakeCode JavaScript. You can also run a local version of the MakeCode online editor (previously known as PXT).

### C/C++

- [C/C++ runtime](https://lancaster-university.github.io/microbit-docs/) - Guidance on how to start using the runtime in C/C++ including full documentation of the APIs, drivers, and types that make up the micro:bit runtime. Bluetooth documentation includes a link to the original `*.hex` file that ships on the micro:bit devices.
- [Arduino nRF5](https://github.com/sandeepmistry/arduino-nRF5/) - Arduino Core for Nordic Semiconductor nRF5 based boards, including the micro:bit.

##### C/C++ Editors

- [Micro:Pi](https://github.com/Bottersnike/Micro-Pi) - C/C++ editor for the micro:bit with serial monitor and deploy functionality. Written in Python with an installer (ATM Linux only, but could be manually installed in any OS) that includes all dependencies.

##### C/C++ Libraries

- [OneWire](https://github.com/adamboardman/microbit-onewire) - BBC micro:bit OneWire Library, based upon Erik Olieman's mbed DS1820 lib.
- [neopixel](https://github.com/elmorg/uBit_neopixel) - Library for using neopixels with the BBC micro:bit.
- [microbit Screen](https://github.com/ht-deko/microbit_Screen) - Arduino LED Screen library for micro:bit.
- [Adafruit Arduino MicroBit library](https://github.com/adafruit/Adafruit_Microbit) - Wrapper code and examples for using micro:bit with Arduino IDE.

### Other micro:bit Languages

- [Touch Develop](https://www.microbit.co.uk/create-code#touchdevelopEditor) - Flexible, text-based programming language with an interactive visual component.
- [Rust on BBC micro:bit](https://github.com/SimonSapin/rust-on-bbc-microbit) - Article describing the experience and steps of compiling Rust code for the micro:bit with and without interaction with the runtime DAL.
- [Forth](https://wiki.forth-ev.de/doku.php/en:projects:microbit:start) - Forth, a stack-based language, for the BBC micro:bit.
- [Pascal](http://wiki.freepascal.org/micro:bit) - Free Pascal compiler that can target the ARM embedded platform, including the micro:bit.
- [Ada](https://github.com/AdaCore/Ada_Drivers_Library/tree/master/examples/MicroBit) - Instruction on how to setup the Ada development environment for the micro:bit.

### Other Interaction Languages

- [Kodu Controller](http://www.kodugamelab.com/bbc-microbit/) - Enables interacting with the microbit from Kodu Game Lab.
- [Simulink Coder Support Package](http://uk.mathworks.com/matlabcentral/fileexchange/60273-simulink-coder-support-package-for-bbc-micro-bit-board) - Package that enables you to create Simulink models and automatically generate and deploy code on the micro:bit.
- [microbit for Dyalog APL on the Pi](https://github.com/APLPi/microbit) - Tools for using the micro:bit (via MicroPython serial connection) with the Dyalog APL programming language on the Raspberry Pi.
- [Gobot](https://gobot.io/documentation/platforms/microbit/) - Framework for the Go programming language to program devices in the real world. It can now the micro:bit via Bluetooth LE.
- [Microbit Unity](https://github.com/bLiGM/Microbit-Unity) - Unity scripts to allow the BBC Microbit to be used as a Unity Controller.
- [Haxe node BBC micro:bit](https://github.com/MatthijsKamstra/hx-node-bbc-microbit) - Control a BBC micro:bit from Node.js using BLE and the Haxe programming language.
- [App Inventor + IoT](http://iot.appinventor.mit.edu/#/microbit/microbitintro) - Control a micro:bit via Bluetooth with App Inventor, a visual programming environment for Android applications.
- [BlockyTalkyBLE](http://www.playfulcomputation.group/blockytalkyble.html) - MakeCode and App Inventor extension that makes it easy to connect AppInventor mobile phone apps with the BBC micro:bit wirelessly over Bluetooth.
- [DroidScript - MicroBit Plugin](https://play.google.com/store/apps/details?id=org.droidscript.microbit) - Allows you you to control the BBC micro:bit remotely from your own DroidScript apps (Android apps written in JavaScript).
- [CBMicroBit](https://github.com/Louismac/CBMicroBit) - CoreBluetooth wrapper in C++ that connects a micro:bit to a computer running OSX using BLE and outputs over OSC (can be used standalone, or as a C++ or Objective C library).


## Programming Tools

- [Vagrant C/C++ Development Environment](https://github.com/carlosperate/microbit-dev-env) - Creates a virtual machine with all the toolchain required to compile and flash C/C++ and MakeCode programs to the micro:bit (including  MicroPython).
- [micro:bit uploader](https://www.touchdevelop.com/microbituploader) - Windows application that monitors your Downloads folder and flashes any new programs to the micro:bit.


## Mobile Apps

- [Official Android App](https://play.google.com/store/apps/details?id=com.samsung.microbit) ([Source Code](https://github.com/Samsung/microbit)) - Pair, program and flash programs to the micro:bit via Bluetooth.
- [Official iOS App](https://itunes.apple.com/gb/app/micro-bit/id1092687276) - Pair, program and flash programs to the micro:bit via Bluetooth.
- [micro:bit Blue](https://play.google.com/store/apps/details?id=com.bluetooth.mwoolley.microbitbledemo) ([Source Code](https://github.com/microbit-foundation/microbit-blue)) - Android app that contains a series demos for interacting with the micro:bit using Bluetooth.
- [Bitty Software Apps](http://www.bittysoftware.com/apps.html) - Diverse collection of Android and iOS apps, going from data logging to audio pranks, you'll certainly find something of interest. 
- [Insight Mr Bit](http://www.insightresources.co.uk/microbit/page63.html) ([iOS](https://itunes.apple.com/gb/app/insight-mr-bit/id1175915875)) - Create simple programs in plain English to control the BBC micro:bit to do lots of useful things.
- [Micro:bit Xamarin](https://play.google.com/store/apps/details?id=com.sumitgouthaman.microbitble) ([Source code](https://github.com/sumitgouthaman/microbit-ble-mobile)) - Android app that demonstrates communicating with BBC micro:bit over Bluetooth LE and getting sensor data. As an open source app, it's a good example of using Xamaring with the micro:bit.
- [bitty blue](http://www.bittysoftware.com/apps/bitty_blue.html) - iOS and Android app that provides a collection of fun things to do with a BBC micro:bit (or compatible device) and Bluetooth.
- [micro:bit logger](https://play.google.com/store/apps/details?id=nl.defbu.mblogger) - Android app that enables users to log data from the BLE services and export it to a file. 


## ChromeOS Apps

- [bitty blue](http://www.bittysoftware.com/apps/bitty_blue.html) - Play with 3D "PolySquiggles", use as a compass, have fun with the buttons, send images or text to the LED display, connect and control electronic circuits, and all via Bluetooth.
- [bitty data logger](http://www.bittysoftware.com/apps/bitty_data_logger.html) - Capture and chart accelerometer, magnetometer and temperature data from your micro:bit's internal sensors over Bluetooth.
- [microbit chrome](https://github.com/Microsoft/microbit-chrome) - Prototype chrome addon that exposes the micro:bit's serial output to webpages like the MakeCode editor.


## Interface Chip

The USB Interface Chip is the microcontroller placed close to the battery connector. It provides the USB mass storage capability to load the micro:bit firmware using the Operating System file explorer.

- [microbit.org Developer Community Info](http://tech.microbit.org/software/daplink-interface/) - This micro:bit Developer Community page contains information about the Interface Chip DAPlink and the USB interface.
- [DAPLink on micro:bit](https://www.mbed.com/en/development/hardware/prototyping-production/daplink/daplink-on-kl26z/) - The DAPLink is the default software running on the Interface Chip, this page contains information, update instructions, and the latest firmware.
- [DAPLink source code](https://github.com/mbedmicro/DAPLink) - Source code for the mbed DAPLink, contains the build configuration for the micro:bit.
- [J-Link OB Firmware](https://www.segger.com/bbc-micro-bit.html) - Offers the same flashing functionality than the DAPLink and expands it to include J-Link debugging.
- [pyOCD](https://github.com/mbedmicro/pyOCD) - Python library for programming and debugging ARM Cortex-M microcontrollers, like the one included in the micro:bit, using the CMSIS-DAP provided by the Interface Chip.
- [DAP.JS](https://github.com/Microsoft/dapjs) - Node.js interface to DAP-CMSIS over USB/HID, meant to provide a subset of functionality of pyOCD.


## Hardware

- [Hardware Design](https://github.com/bbcmicrobit/hardware) - Schematics and bill of materials for the BBC micro:bit.
- [micro:bit Reference Design](https://github.com/microbit-foundation/microbit-reference-design) - Hardware design files for a board 100% binary compatible with the micro:bit. Created to help make your own micro:bit derived designs.
- [micro:bit Badge](https://github.com/make-zurich/micro-bit-badge) - Open Source PCB for the micro:bit with a battery holder, buzzer, extension edge connector and pins breaks out.
- [Eagle micro:bit Edge Part](https://github.com/proto-pic/micro-bit-eagle-libraries) - Eagle librarie from Proto-Pic for the micro:bit edge connectors.
- [Kicad micro:bit Connector](https://github.com/anthonykirby/kicad_microbit_connector) - KiCad component library and footprint library for a micro:bit edge-connector socket.
- [SparkFun Breakout Board](https://github.com/sparkfun/Micro_Bit_Breakout) - Open source files for the SparkFun micro:bit Breakout Board.
- [SparkFun moto:bit](https://github.com/sparkfun/Micro_Bit_Moto_Bit) - Open source files for the SparkFun moto:bit, a board to provide a robotics platform,
- [SparkFun weather:bit](https://github.com/sparkfun/Micro_Bit_Weather_Bit) - Open source files for the SparkFun weather:bit, a board to provide a weather station.
- [SparkFun gamer:bit](https://github.com/sparkfun/Micro_Bit_Gamer_Bit) - Open source files for the SparkFun gamer:bit, a board to provide a game system.


## CAD & 3D Printing

- [Kitronik CAD Resources](https://www.kitronik.co.uk/blog/bbc-microbit-cad-resources/) - BBC micro:bit CAD model from Kitronik.
- [Proto-PIC CAD Resources](https://www.proto-pic.co.uk/micro-bit-resources.html) - Proto-PIC products CAD resources.
- [Microbot Case](http://www.thingiverse.com/thing:1434797) - 3D printed case for the micro:bit in the shape of a robot.
- [micro:bit Stand](http://www.thingiverse.com/thing:2144500) - 3D printed stand for the micro:bit.
- [micro:bit Rover](https://www.myminifactory.com/object/microbit-rover-27013) - 3D printable parts to build a micro:bit robot rover.
- [Micro:Racing](https://www.myminifactory.com/object/micro-racing-18280) - 3D printed wheel case for the micro:bit.
- [Binary Watch](https://www.myminifactory.com/object/binary-watch-15257) - 3D printed watch case and strap for the micro:bit.
- [Micro:bit Compass](https://www.myminifactory.com/object/micro-bit-compass-18994) -3D printed compass case for the micro:bit.
- [A4 folder holder](https://www.myminifactory.com/object/micro-bit-a4-folder-holder-22039) - 3D printed holder to keep your micro:bit in a A4 school folder.
- [mibot drawing robot](https://www.myminifactory.com/object/mibot-drawing-robot-36030) - 3D printed chassis for a painting robot powered by a BBC micro:bit and its motor drive board.


## Projects

All these projects contain steps and resources required for reproduction.

- [Quiz:bit](https://github.com/lancaster-university/quiz-bit) - BBC micro:bit programs and a matching application for providing a quiz-voter-style service using micro:bits as the controls.
- [JUST DO IoT](https://hackaday.io/project/12164-just-do-iot) - Connect the micro:Bit to the LoRaWAN network, includes open source hardware microbit connector board.
- [Micro:Bob](https://hackaday.io/project/8643-microbob) - Simple bipedal robot controlled by a micro:bit.
- Coffee Timer ([1](https://www.norwegiancreations.com/2016/09/coffee-timer-part-1-the-first-prototype-based-on-the-bbc-microbit/), [2](https://www.norwegiancreations.com/2016/10/coffee-timer-part-2-low-power-wireless-on-the-bbc-microbit/), [3](https://www.norwegiancreations.com/2016/11/coffee-timer-part-3-enclosures/)) - Three part article describing how to augment a coffee maker with an micro:bit indicator, options for low power communication, and creating a custom enclosure.
- [Thermal Printer](http://www.suppertime.co.uk/blogmywiki/2016/12/microbit-thermal/) - Connecting and using a Sparkfun thermal till-roll printer.
- [Telescopic Light Sword](https://www.myminifactory.com/object/telescopic-lightsword-with-micro-bit-14598) - Project shows how to make your own Light Sword with the micro:bit, electronics, and 3D printed parts.
- [Micro Simon](http://mrtomsworld.blogspot.co.uk/2017/01/micro-simon.html) - Programming and connecting a micro:bit to a vintage MB Simon game.
- [Connecting a thermal printer to a BBC microbit](http://www.suppertime.co.uk/blogmywiki/2016/12/microbit-thermal/) - Connecting the micro:bit to a thermal till-roll printer to print a random poems or Christmas cracker jokes.
- [Alexa Weather On micro:bit](https://www.hackster.io/chen-tiebiao/weather-on-micro-bit-c79c19) - Creating an Amazon Alexa skill where the current weather can be asked and the result displayed on the micro:bit.
- [BBC Microbit Balloon Tracker](http://www.daveakerman.com/?p=2019) - Making a ballon tracker with a micro:bit connected to GPS and a LoRa transceiver to track and transmit its position.
- [SonicPixels](https://github.com/jrmedd/SonicPixels) - BBC micro:bit and Max frameworks for triggering multiple speakers in a grid arrangment.
- [Little Bug Bit](http://goo.gl/eEFhcy) - Low cost micro:bit buggy.
- [HandShake](https://sites.google.com/site/hardwaremonkey/home/handshake) - Project designed to enable unique gesture recognition for people with limited control of their motion.
- [Mega:Bit](http://www.makerspace-uk.co.uk/megabit/) - Scaled up micro:bit with the 5x5 LED matrix and buttons, connected to a real micro:bit.
- [Scrolling display](https://meanderingpi.wordpress.com/2017/09/16/bbc-microbit-scrolling-display/) - Create a display screen using a number of micro:bits communicating via radio.
- [Ironman Arc Reactor](https://www.kitronik.co.uk/blog/halo-ween-ironman-arc-reactor) - Choose between two different versions (Mk I and Mk II) ready to 3D print and build.

### Project Collections

- [microbit.co.uk Site Index](https://www.microbit.co.uk/index) - The microbit.co.uk website contains an extensive list with all their projects and tutorials.
- [hackster micro:bit community](https://www.hackster.io/micro-bit/projects) - This hackster community contains user submitted projects for the micro:bit.
- [MakeCode Projects](https://makecode.microbit.org/projects/) - List of micro:bit projects you can do with the MakeCode editor.
- [Inventorspace micro:bit category](https://invent.sparkfun.com/cwists/category#products=%5B8%5D) - Community by SparkFun with fun projects you can implement in your classroom, school or district.
- [Tinkercademy Projects](https://tinkercademy.com/microbit/) - Collection of projects using the micro:bit and Tinkercademy Tinker Kit.


## Articles

Useful Articles for developing on the micro:bit.

- [Getting Started Microbit & Microsoft’s new www.codethemicrobit.com Environment](https://blogs.msdn.microsoft.com/uk_faculty_connection/2016/08/01/getting-started-microbit-microsofts-new-www-codethemicrobit-com-environment/)
- [Offline C/C++ Development With The Micro:bit](http://www.i-programmer.info/programming/hardware/9654-offline-cc-development-with-the-microbit-.html)
- [Sending 'commands' from a micro:bit over Bluetooth](http://bluetooth-mdw.blogspot.co.uk/2016/07/sending-commands-from-microbit-over.html)
- [Modelling micro:bit data with the Bitty Data Logger App](https://www.stem.org.uk/elibrary/community-resource/289686/modelling-microbit-data-bitty-data-logger-app)
- [Getting Started with the micro:bit Bluetooth IO Pin Service](https://ukbaz.github.io/howto/ubit_ble_profile.html)
- [Using MQTT-SN over BLE with the BBC micro:bit](https://blog.benjamin-cabe.com/2017/01/16/using-mqtt-sn-over-ble-with-the-bbc-microbit)
- [The First Video Game on the BBC Micro:bit [probably]](https://hackernoon.com/the-first-video-game-on-the-bbc-micro-bit-probably-4175fab44da8) - Creating a game for the micro:bit, the MicroPython changes needed to increase performance and a general profile of its resources.
- [Custom BLE services with micro:bit](https://www.hackster.io/pelikhan/custom-ble-services-with-micro-bit-6c9879) - Build your own Bluetooth low energy services and bundle them as PXT/MakeCode blocks that beginners can use.
- [Excel and Micro:Bit - Hacking for fun and creativity!](https://techcommunity.microsoft.com/t5/Excel-Blog/Excel-and-Micro-Bit-Hacking-for-fun-and-creativity/ba-p/63603) - Experiment to have some basic sensor data collected using the micro controller and then visualized in Excel.
- [Writing the second video game for the Micro:bit in Rust](https://hackernoon.com/writing-the-second-video-game-for-the-micro-bit-in-rust-3cd8b5ab22d3) - Updating a micro:bit game and porting it to the Rust language.
- [Build A Klawsome microbit Controlled Tank](https://www.kitronik.co.uk/blog/klawsome-microbit-controlled-tank/) - Tutorial on how to design a build a perspex micro:bit tank.
- [Adding a new module to MicroPython](http://cigdemsengul.blogspot.co.uk/2017/04/offline-development-in-microbit-adding.html) - Article describing an experiment to add a new module into MicroPython for the micro:bit.
- [Become a Time Lord with the BBC micro:bit](https://blog.groklearning.com/become-a-time-lord-with-the-bbc-micro-bit-c4b8b4e2d747) - Using different timing mechanisms to run multiple things in MicroPython.
- [Debugging the micro:bit with pyOCD and GDB](https://docs.mbed.com/docs/mbed-os-handbook/en/5.4/debugging/debugging_microbit/) - Shows how to debug a micro:bit program using PyOCD and GDB.

### Article Collections

- [MultiWingSpan](http://www.multiwingspan.co.uk/micro.php) - Large collection of examples, instructions, and direction on how to use electronic components.
- [Elecfreaks micro:bit category](https://www.elecfreaks.com/category/micro-bit) - Elecfreaks collection of experiments going through the concepts of using individual sensors or components.
- [SparkFun micro:bit tutorials](https://learn.sparkfun.com/tutorials/tags/microbit) - Collection of tutorials from SparkFun, including comprehensive experiment guides for their kits.
- [BitIO blogs](http://warksjammy.blogspot.co.uk/2017/07/bitio-blogs-in-one-place.html) - Collection of blogs written about using the BitIO Python module to control the micro:bit. 


## Videos

- [MicroMonsters](https://www.youtube.com/channel/UCK2DviDexh_Er2QYZerZyZQ) - YouTube channel with tutorials to learn to code with your family.
- [micro:bit and Bluetooth](https://www.youtube.com/playlist?list=PLYOCnwH2UtBzhJ2nvn_DM3itz6GNVwrDu) - YouTube playlist with Martin Woolley's Bluetooth videos.
- [Video Series from The Maker Movies](https://www.youtube.com/playlist?list=PLD0HD_3AJljXDWoasq2x5gHmkKeV7cc-P) - List of short, introductory videos for anyone wanting to get started with the micro:bit.
- [SparkFun video resources](http://sparkfuneducation.com/video-resources/microbit.html) - Growing list of video resources for the micro:bit.
- [SamCodes YouTube Playlist](https://www.youtube.com/playlist?list=PLumNlyd5JxxegaAVScP7Qm1AXPtJdGBCq) - Video tutorials showing how to  use different electronic components and features of the micro:bit.
- [Fun with Zephyr Project and BBC micro:bit](https://www.youtube.com/watch?v=ZZRbIpVJGns) - This presentation shows how Zephyr empowers the BBC micro:bit devices and its Bluetooth chip to do fun things.


## Books

- [micro:bit IoT In C](http://www.iot-programmer.com/index.php/books/micro-bit-iot-in-c)
- [BBC micro:bit - 35 Touch Develop & MicroPython Projects](https://www.elektor.com/bbc-micro-bit-35-touch-develop-micropython-projects)
- [Programming with MicroPython](http://shop.oreilly.com/product/0636920056515.do)
- [Getting Started with the micro:bit](http://shop.oreilly.com/product/0636920115267.do)
- [The Official BBC micro:bit User Guide](http://eu.wiley.com/WileyCDA/WileyTitle/productCd-111938673X.html)
- [Programming the BBC micro:bit](http://simonmonk.org/prog_mb/)


## Teaching Resources

- [microbit.org Teaching Resources](https://www.microbit.org/teach/)
- [IET micro:bit Teaching Resources](http://faraday.theiet.org/stem-activity-days/bbc-microbit/resources/index.cfm)
- [Code Club micro:bit projects](https://www.codeclubprojects.org/en-GB/microbit/)
- [Make with the micro:bit by Technology Will Save Us](http://make.techwillsaveus.com/bbc-microbit)
- [Grok Learning](https://groklearning.com/microbit/) - Provides an online MicroPython code editor, Blockly visual programming, full micro:bit simulator, curriculum-aligned teaching material and auto-marked problems.
- [Microbit For Primary Schools](http://mb4ps.co.uk) - Fully-customisable scheme of work and resources for use in the primary classroom. 
- [101 Computing BBC micro:bit category](http://www.101computing.net/category/bbc-microbit/) - Computing challenges with the micro:bit to boost your programming skills or spice up your teaching of computer science.
- [Micro:bit Maths](https://microbitmathsblog.wordpress.com) - Blog exploring the BBC micro:bit in mathematics education.
- [micro:bit of Things](https://sites.google.com/view/microbitofthings/) - Notes on micro:bit project ideas for Key Stage 2 and 3.
- [The Brooke Primary School Space Programme](http://www.brooke.norfolk.sch.uk/brooke-space-programme/) - Project page documenting Brooke Primary School pupil's upcoming journey for launching a BBC micro:bit (on its own) into near-space, with experiments and sensor measurements.
- [FunWithMicrobit](https://github.com/MicrobitPolska/FunWithMicrobit) - FunWithMicrobit is a 6 hours workshop made by kids for the kids.
- [Year 7 micro:bit lessons](http://www.jonwitts.co.uk/year-7-microbit) - Lessons used to introduce students to the micro:bit and Python.
- [UCL’s BBC Micro:bit Tutorials](http://microbit-challenges.readthedocs.io/en/latest/) - Tutorial sheets that introduce micro:bit features with practical examples provided to invite students to design solutions to problems.
- [BBC micro:bit and Kodu Interact](https://www.kodugamelab.com/resources/#microbit) - Kodu is a visual programming language made specifically for creating games and allow interaction with the micro:bit.
- [Build A Robot Wars Buggy](https://www.kitronik.co.uk/blog/robot-buggy-part-1-build-robot-wars-buggy-introduction/) - This fun learning resource has been put together to provide teachers with an all in one design and technology challenge that you can set for your students over the course of a term or a year.
- [CPC UCreate Micro:bit resources](http://warksjammy.blogspot.co.uk/2017/04/cpc-ucreate-microbit-resources-all-in.html) - Collection of micro:bit resources made for CPC.
- [Year 7 BBC micro:bit topic](https://bournetocode.com/projects/7-CS-micro/) - BBC micro:bit lessons from Bourne Grammar school.
- [Doctor Who Live Lesson](http://www.bbc.co.uk/programmes/articles/3ydvd6mvhl89cHVJ7F2nmzf/doctor-who-and-the-micro-bit-live-lesson) - The BBC micro:bit will be put to the test at the controls of the TARDIS in this special BBC Live Lesson in collaboration with the team behind Doctor Who.
- [Tackle time and space with Doctor Who and the BBC micro:bit](http://www.bbc.co.uk/programmes/articles/GDNGTpkHJrDJSYMQJbH9f1/tackle-time-and-space-with-doctor-who-and-the-bbc-micro-bit) - Join The Doctor on an adventure of courage, cunning and coding! Part 1: Mission Sonic, Part 2: Mission Decode, and Part 3: Mission Hack.
- [Microsoft 14 Week Curriculum](https://makecode.microbit.org/courses/csintro) - Targeted to middle school grades 6-8 (ages 11-14 years). It is also written for teachers who may not have a Computer Science background, or may be teaching an "Intro to CS" for the first time.
- [micro:bit in science teaching - How clean is my pond](https://community.computingatschool.org.uk/resources/5204) - Using a micro:bit to monitor the level of algal growth in a pond and to control a filter pump.
- [Inventorspace micro:bit category](https://invent.sparkfun.com/cwists/category#products=%5B8%5D) - Community by SparkFun with fun projects you can implement in your classroom, school or district.
- [Strictly micro:bit - BBC Live Lessons](https://www.youtube.com/watch?v=QgEP8aI8Gvw&index=1&list=PLcvEcrsF_9zL-zmL_1-yikUGtsTMo1oO-) - Suitable for teaching ages 11-14. The full BBC Live Lesson exploring the basics of coding, with help from the stars of Strictly Come Dancing and the BBC micro:bit.


## Community

- [Official Slack Channel](http://tech.microbit.org/get-involved/where-to-find/) - Online form to join this chat group, a great place to discuss and meet more people from the micro:bit community.
- [`@microbit_edu` on twitter](https://twitter.com/microbit_edu)
- [`microbitfoundation` on Facebook](https://www.facebook.com/microbitfoundation)
- [micro:bit Python mailing list](https://mail.python.org/mailman/listinfo/microbit)


## Miscellaneous

- [microbit Fritzing Part](https://github.com/topshed/FritzingParts) - Richard Hayler collection of Fritzing parts contains a model for the micro:bit.
- [micro:bit broadcast](https://microbit-broadcast.embeddedlog.com) - Free newsletter to stay up-to-date with the latest micro:bit news, articles, projects, and resources.
- [micro:bit-o-matic](https://pycomic.github.io/microbit.html) - Easily create micro:bit illustrations with custom LED matrix messages.
- [microbit.org Support](https://support.microbit.org) - The support pages from the micro:bit Foundation is a great source of information, containing an extensive collection of FAQs, articles, and guides. 
- [Radiobit, a BBC Micro:Bit RF firmware](https://github.com/virtualabs/radiobit) - Radiobit is composed of a dedicated Micropython-based firmware and a set of tools allowing security researchers to sniff, receive and send data over Nordic's ShockBurst protocol, Enhanced ShockBurst protocol, Bluetooth Smart Link Layer and sniff raw 2.4GHz GFSK demodulated data.
- [micro:bit Poster](https://www.element14.com/community/servlet/JiveServlet/downloadBody/87638-102-3-368412/microbit24x15.pdf) - Element14 has put together this detailed, beautifully rendered, cross-section micro:bit poster highlighting all of the device's key functions and components.
- [Bluetooth troubleshooting guide](http://www.bittysoftware.com/troubleshooting.html) - Tips on how to solve common and not so common micro:bit Bluetooth problems.
- [Micro World Tour](https://microworldtour.github.io) - Before the micro:bit was released a few went on a tour to the world-wide Python community. A lot of interesting content and ideas on these micro:bit adventures.


## License & Trademarks

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the authors have waived all copyright and related or neighbouring rights to this work.

This projects is not endorsed, sponsored or associated with the BBC. "BBC", "micro:bit", and their logos are trademarks of the BBC.
