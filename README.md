# Overview

This project is my first attempt at building a portable cyberdeck using a Raspberry Pi 4 and a Pelican 1150 case. It’s designed to be fully self-contained, with water-resistant ports, onboard battery power, and cooling fans. My main focus was to create a sleek, functional system for running various scripts and tasks, such as BadUSB attacks, while keeping everything compact and portable.
In the future I plan to add assembly instructions and electrical shcematics.

![Cyberdeck Build](https://i.imgur.com/6F71S5s.jpeg)

---

## Features
- **7-inch display**: Built-in for portable use
- **Running Kali Linux**: Ideal for cybersecurity tasks
- **Active cooling system**: 1x 30mm fan and 2x 18mm fans provide airflow when the case is open
- **3 USB ports**: 2 internal, 1 external for peripherals
- **SD card reader**: Built-in for easy storage access
- **HDMI output**: External port for connecting to a larger display
- **USB-C charging**: Convenient power supply for both the Pi and the screen
- **Cat5 Ethernet port**: External network connection for wired access
- **Audio jack**: For headphones or external audio
- **Status LEDs**:
  - Charging indicator
  - Raspberry Pi on/off
  - Screen on/off
  - 3 additional customizable LEDs
- **Switch for screen power**: Automatically turns the screen off when the case is closed
- **Keyboard**: Integrated for ease of use
- **Storage compartments**: Holds SD cards and USB drives under the keyboard
- **Fully-contained battery**: Powers both the Raspberry Pi and screen for portable operation
- **Water-resistant design**: Sealed and protected when closed

---

## Known Issues
- **Overheating**: Cannot operate with the lid closed for extended periods due to heat buildup
- **No trackpad**: There's no way to control the cursor in the OS without an external mouse
- **Boot issue**: Raspberry Pi won’t boot from the SD card reader
- **Status LEDs**: The LEDs are too bright (can be fixed by using different resistors)
- **Charging inconvenience**: The keyboard has to be removed to access the charging port
- **Internal cable management**: Very poor, leading to a cluttered interior
- **Waterproofing**: The build does not maintain the Pelican case’s original waterproof rating
- **Glue used for assembly**: Insert/faceplate is fastened using glue, which could be improved
- **Charging limitations**: Only supports standard USB charging, not USB-C PD; USB-C port is not bi-directional (input only)

---

## Future Goals
- **Custom 18650 battery pack**: Build a battery pack to fit the case better, provide a longer runtime, and support USB-C PD input and output
- **Slightly bigger case**: Upgrade to a larger case for better component fit and expansion
- **New cooling design**: Implement a thermoelectric cooling system to allow operation with the lid closed
- **Add a trackpad**: Include a built-in trackpad for easier navigation
- **Improved waterproofing**: Enhance external I/O with more waterproof options
- **Upgrade to Raspberry Pi 5**: Consider switching to a Raspberry Pi 5 for improved performance
- **Use fasteners instead of glue**: Replace glued components with screw fasteners for a cleaner, more durable assembly
- **Use SSD for booting**: Switch to an SSD for faster and more reliable booting
- **Design custom PCB**: Create a custom PCB for improved wire management and cleaner internal layout
- **More improvements to come**: This project is evolving, and additional upgrades are planned for future versions

---

## Parts List

#### Disclaimer
Some of the links may have changed, so the parts may not be *identical*. Everything looks the same on the listings, but these parts were all ordered over a year ago.

---

#### Case and External I/O

- **Pelican Case**: [Pelican 1150 Case](https://shorturl.at/xyr0k)
- **Water-resistant Panel Mount I/O (sold by Power Signal Data Connector Store on AliExpress)**:
  - [External HDMI Port](https://shorturl.at/CyrGC)
  - [External USB Port](https://shorturl.at/Cf8bj)
  - [External USB-C Port](https://shorturl.at/6hTVx)
  - [External RJ45 Port](https://shorturl.at/9zwq1)

  These can be ordered in any color and configuration, but I ordered mine in black with metal nuts. All connectors are ports, but soldering versions are available.

---

#### Display and Input

- **Display**: [7-inch 1024x600 HDMI Display](https://shorturl.at/NZxAf)
- **Keyboard**: [7-inch Tablet Keyboard](https://a.co/d/doeQoq1) – You can also find versions with a trackpad, but the keyboard base may need modification.
- **3.5mm Audio Jack**: [Panel Mount 3.5mm Audio Jack (3-pin)](https://shorturl.at/4XXrT)

---

#### Cooling and Switches

- **Fans**:
  - [30mm Fan (5V)](https://shorturl.at/P3yWi)
  - [20mm Fan (5V Hydraulic Bearing)](https://a.co/d/7ztwXzH)
- **Rocker Switches**: [Small Round 2-pin Rocker Switches](https://shorturl.at/hRt7r)
- **Lid Switch**: [Refrigerator Door Light Switch (Normally Closed)](https://a.co/d/ivMNV4H) or [Alternative Link](https://shorturl.at/g9zLX)

---

#### Internal Components

- **Internal USB Ports**: [USB to USB 3.0 Dual Panel Mount](https://a.co/d/hqzMyTw)
- **SD Card Extender**: [Micro SD to SD Card Extender](https://shorturl.at/vaQC8)
  > Note: For some reason, the Pi won't boot from an SD card plugged into this. I'm currently using it with a USB to Micro-USB adapter for reading SD cards, but it works intermittently. You may want to find an alternative.
- **Brass Standoffs**: [Brass Standoffs](https://shorturl.at/BhvH3) – Any small standoff that fits the Pi’s holes should work fine. I inserted mine into the 3D printed part using a soldering iron. Dimensions: box part is 4.8mm tall, 4.5mm wide; shaft is 5mm long, 2.5mm wide.

---

#### LEDs and Power

- **LEDs and Resistors**:
  - [5mm LEDs](https://shorturl.at/MhEKz) – Any standard 5mm LED will work; mine were pulled from a DIY Pi kit.
  - [390 Ohm Resistors](https://shorturl.at/njeu3) – Used for the LEDs. You may want to use a higher resistance as these are quite bright.
- **Diode**: [3A Diode (supports 5V)](https://a.co/d/aqU21aW) – This is used to prevent the charging LED from being powered by the battery bank, so it only turns on during charging. This setup prevents the USB-C port from being used as a power source, as noted in the issues section.

---

#### Cables and Wiring

- **Cables**:
  - [Micro HDMI to HDMI](https://shorturl.at/lDclC)
  - [Micro HDMI to Mini HDMI](https://a.co/d/1WwkHYU)
  - [USB A to USB A](https://shorturl.at/Ay4hM) – I made my own, but this should work.
  - [RJ45 Male to RJ45 Male](https://shorturl.at/zojFO) – I made my own, but this should work.
- **Wiring and Heatshrink**: I used spare 22AWG wire and heatshrink, but you can find similar materials [here](https://shorturl.at/3O9jX) and [here](https://shorturl.at/ypX5P) for the USB-C and micro USB connections (Pi, screen, and charging). You may need some non-USB-C PD cables and ends to solder up.

---

#### 3D Printed Parts

- **3D Printed Components**: All parts are printed with **Polymaker PETG**, but any standard filament should work.
****

