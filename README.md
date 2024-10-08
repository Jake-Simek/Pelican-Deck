# Overview

This project is my first attempt at building a portable cyberdeck using a Raspberry Pi 4 and a Pelican 1150 case. It’s designed to be fully self-contained, with water-resistant ports, onboard battery power, and cooling fans. My main focus was to create a sleek, functional system for running various scripts and tasks, such as BadUSB attacks, while keeping everything compact and portable.

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

