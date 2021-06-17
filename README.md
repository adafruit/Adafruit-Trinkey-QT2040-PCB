## Adafruit Trinkey QT2040 PCB

<a href="http://www.adafruit.com/products/5056"><img src="assets/5056.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit Trinkey QT2040. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5056

### Description

It's half USB Key, half Adafruit QT Py, and a lotta RP2040...it's Trinkey QT2040, the circuit board with an RP2040 heart and Stemma QT legs. Folks are loving the QT Py 2040 we made, but maybe you want something plug-and-play. So we thought, hey what if we made something like that plugs right into your computer's USB port? And this is what we came up with!

The PCB is designed to slip into any USB A port on a computer or laptop. There's an RP2040 microcontroller on board with just enough circuitry to keep it happy. There's an RGB NeoPixel, a reset and bootloader or user button and a STEMMA QT Port on the end. That's it!

With the body of the board being 1.0" x 0.7" and four mounting holes, you can attach just about any of our QT boards right on (some are a little larger so just check that has the holes in the same locations). Use M2.5 sized standoffs and screws to do so, you could use 2 diagonal at a minimum. Then use a shorty QT cable and you've got a custom sensor Trinkey for any sensor purpose.

The board comes with 8 MB of QSPI flash memory so you can put all of our CircuitPython drivers on the disk!

#### Plug-and-play STEMMA QT

One of the stars of this board is our favorite connector - the STEMMA QT, a chainable I2C port that can be used with any of our STEMMA QT sensors and accessories. Having this connector means you don't need to do any soldering to get started.

What can you pop into the QT port? How about OLEDs! Inertial Measurement Units! Sensors a-plenty. All plug-and-play thanks to the innovative chainable design: SparkFun Qwiic-compatible STEMMA QT connectors for the I2C bus so you don't even need to solder. Just plug in a compatible cable and attach it to your MCU of choice, and you’re ready to load up some software and measure some light.

Use any SparkFun Qwiic boards! Seeed Grove I2C boards will also work with this adapter cable.

#### Software Support

At the time of launch, there is no Arduino core support for the chip on this board. There is great C/C++ support, an official MicroPython port, and a CircuitPython port! We of course recommend CircuitPython because we think it's the easiest way to get started and it has support with most of our drivers, displays, sensors, and more, supported out of the box so you can follow along with our CircuitPython projects and tutorials.

While the RP2040 has lots of onboard RAM (264KB), it does not have built-in FLASH memory. Instead, that is provided by the external QSPI flash chip. On this board there is 8MB, which is shared between the program it's running and any file storage used by MicroPython or CircuitPython. When using C/C++ you get the whole flash memory, if using Python you will have about 7 MB remaining for code, files, images, fonts, etc.

* Main body is same size/mounting holes as most of our Stemma QT boards (1.0" x 0.7" with M2.5 holes)
* USB Type A connector with extra-thick PCB to fit into a USB host port
* RP2040 32-bit Cortex M0+ dual-core running at ~125 MHz @ 3.3V logic and power
* 264 KB RAM
* 8 MB SPI FLASH chip for storing files and CircuitPython/MicroPython code storage. No EEPROM
* Native USB supported by every OS - can be used as USB serial console, MIDI, Keyboard/Mouse HID, even a little disk drive for storing Python scripts.
* Can be used with MicroPython or CircuitPython
* Built-in RGB NeoPixel LED
* STEMMA QT / Qwiic port for I2C connectivity
* 3.3V regulator with 600mA peak output
* 12 MHz crystal
* Both Reset button and Bootloader select buttons for quick restarts (no unplugging-replugging to relaunch code)
* Bootloader button can also be safely used in 'user' code

#### About the RP2040

Inside the RP2040 is a 'permanent ROM' USB UF2 bootloader. What that means is when you want to program new firmware, you can hold down the BOOT button while plugging it into USB (or pulling down the RUN/Reset pin to ground) and it will appear as a USB disk drive you can drag the firmware onto. Folks who have been using Adafruit products will find this very familiar - we use the technique on all our native-USB boards. Just note you don't double-click reset, instead hold down the BOOT button during boot to enter the bootloader!

The RP2040 is a powerful chip, which has the clock speed of our M4 (SAMD51), and two cores that are equivalent to our M0 (SAMD21). Since it is an M0 chip, it does not have a floating point unit or DSP hardware support - so if you're doing something with heavy floating point math, it will be done in software and thus not as fast as an M4. For many other computational tasks, you'll get close-to-M4 speeds!

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
