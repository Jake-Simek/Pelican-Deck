# Overview

This project is my first attempt at building a portable cyberdeck using a Raspberry Pi 4 and a Pelican 1150 case. It’s designed to be fully self-contained, with water-resistant ports, onboard battery power, and cooling fans. My main focus was to create a sleek, functional system for running various scripts and tasks, such as BadUSB attacks, while keeping everything compact and portable.
In the future, I plan to add assembly instructions and electrical schematics.

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

- **Pelican Case**: [Pelican 1150 Case](https://shorturl.at/xyr0k) or [alternative link](https://www.pelican.com/us/en/product/cases/protector/1150/)
- **Water-resistant Panel Mount I/O (sold by [Power Signal Data Connector Store](https://www.aliexpress.com/store/1102188024) on AliExpress)**:
  - [External HDMI Port](https://shorturl.at/CyrGC) or [alternative link](https://www.aliexpress.us/item/3256804676511038.html?spm=a2g0o.cart.0.0.562938da9tuzdT&mp=1&gatewayAdapt=glo2usa)
  - [External USB Port](https://shorturl.at/Cf8bj) or [alternative link](https://www.aliexpress.us/item/3256805021108099.html?spm=a2g0o.detail.0.0.7f3fH9ZSH9ZSXv&mp=1&gatewayAdapt=glo2usa)
  - [External USB-C Port](https://shorturl.at/6hTVx) or [alternative link](https://www.aliexpress.us/item/3256804676644038.html?spm=a2g0o.detail.0.0.3261xuXIxuXIZe&mp=1&gatewayAdapt=glo2usa)
  - [External RJ45 Port](https://shorturl.at/9zwq1) or [alternative link](https://www.aliexpress.us/item/3256805248603359.html?spm=a2g0o.detail.0.0.6504P2iMP2iMBi&mp=1&gatewayAdapt=glo2usa)

  These can be ordered in any color and configuration, but I ordered mine in black with metal nuts. All connectors are ports, but soldering versions are available.

---

#### Display and Input

- **Display**: [7-inch 1024x600 HDMI Display](https://shorturl.at/NZxAf) or [alternative link](https://www.aliexpress.us/item/3256806868466798.html?pdp_npi=4%40dis%21USD%21US%20%2444.80%21US%20%2422.40%21%21%21314.42%21157.21%21%402103340717283966818035330d03eb%2112000039248340416%21sh%21US%214391796073%21X&spm=a2g0o.store_pc_home.allitems_choice_2005636386515.1005007054781550&gatewayAdapt=glo2usa)
- **Keyboard**: [7-inch Tablet Keyboard](https://a.co/d/doeQoq1) or [alternative link](https://www.amazon.com/dp/B088ZWT5N1?ref=cm_sw_r_cp_ud_dp_W3J2JXD4Q4X6JF7ZAZNS_1&ref_=cm_sw_r_cp_ud_dp_W3J2JXD4Q4X6JF7ZAZNS_1&skipTwisterOG=1&th=1)
 – You can also find versions with a trackpad, but the keyboard base may need modification.
- - **3.5mm Audio Jack**: [Panel Mount 3.5mm Audio Jack (3-pin)](https://shorturl.at/4XXrT) or [alternative link](https://www.aliexpress.us/item/3256805998541350.html?spm=a2g0o.order_list.order_list_main.102.61621802XBqfx4&gatewayAdapt=glo2usa)

---

#### Cooling and Switches

- **Fans**:
  - [30mm Fan (5V)](https://shorturl.at/P3yWi) or [alternative link](https://www.aliexpress.us/item/3256806120222119.html?spm=a2g0o.productlist.main.3.3bea380ezXkHoD&algo_pvid=087d325e-d732-40f2-a44e-e86344cc06df&algo_exp_id=087d325e-d732-40f2-a44e-e86344cc06df-1&pdp_npi=4%40dis%21USD%214.57%214.57%21%21%214.57%214.57%21%402101e07217283972539762667ebae0%2112000036695416046%21sea%21US%214391796073%21X&curPageLogUid=BouIf6woF0SP&utparam-url=scene%3Asearch%7Cquery_from%3A)
  - [20mm Fan (5V Hydraulic Bearing)](https://a.co/d/7ztwXzH) or [alternative link](https://www.amazon.com/dp/B08MKVSKR6?ref=cm_sw_r_cp_ud_dp_9MMJGZ18CV85JV7A95QX&ref_=cm_sw_r_cp_ud_dp_9MMJGZ18CV85JV7A95QX&social_share=cm_sw_r_cp_ud_dp_9MMJGZ18CV85JV7A95QX&skipTwisterOG=1&th=1)
- **Rocker Switches**: [Small Round 2-pin Rocker Switches](https://shorturl.at/hRt7r) or [alternative link](https://www.aliexpress.us/item/3256807356199141.html?spm=a2g0o.productlist.main.33.549f33b6wGvfeH&algo_pvid=c1a7f8c8-39f6-425d-ae84-71ed4f782a00&algo_exp_id=c1a7f8c8-39f6-425d-ae84-71ed4f782a00-16&pdp_npi=4%40dis%21USD%212.71%211.56%21%21%2118.99%2110.92%21%402103205217283968820746597e8f89%2112000041227080248%21sea%21US%214391796073%21X&curPageLogUid=bANHgWR5Z65P&utparam-url=scene%3Asearch%7Cquery_from%3A)
- **Lid Switch**: [Refrigerator Door Light Switch (Normally Closed)](https://a.co/d/ivMNV4H) or [alternative link](https://shorturl.at/g9zLX)

---

#### Internal Components

- **Internal USB Ports**: [USB to USB 3.0 Dual Panel Mount](https://a.co/d/hqzMyTw) or [alternative link](https://www.amazon.com/dp/B09QQJJML1?ref=cm_sw_r_cp_ud_dp_K7BSMTF40C3JCCPVZWPJ&ref_=cm_sw_r_cp_ud_dp_K7BSMTF40C3JCCPVZWPJ&social_share=cm_sw_r_cp_ud_dp_K7BSMTF40C3JCCPVZWPJ&skipTwisterOG=1)
- **SD Card Extender**: [Micro SD to SD Card Extender](https://shorturl.at/vaQC8) or [alternative link](https://www.aliexpress.us/item/3256803938544773.html?spm=a2g0o.productlist.main.7.551754d9Y1xT5D&algo_pvid=c2f11514-59ba-42cf-9626-3993c9cf9a8f&aem_p4p_detail=202410080727033596893120997910022643752&algo_exp_id=c2f11514-59ba-42cf-9626-3993c9cf9a8f-3&pdp_npi=4%40dis%21USD%213.60%213.60%21%21%213.60%213.60%21%402101fb1017283976237505258e037e%2112000028118186972%21sea%21US%214391796073%21X&curPageLogUid=1OrPtSy9lcx2&utparam-url=scene%3Asearch%7Cquery_from%3A&search_p4p_id=202410080727033596893120997910022643752_1)
  > Note: For some reason, the Pi won't boot from an SD card plugged into this. I'm currently using it with a USB to Micro-USB adapter for reading SD cards, but it works intermittently. You may want to find an alternative.
- **Brass Standoffs**: [Brass Standoffs](https://shorturl.at/BhvH3) or [alternative link](https://www.aliexpress.us/item/2251832748907515.html?spm=a2g0o.productlist.main.1.77cd124b3Mgj8F&algo_pvid=5a9814cc-31e1-4016-9e33-5ca2258e73d7&algo_exp_id=5a9814cc-31e1-4016-9e33-5ca2258e73d7-0&pdp_npi=4%40dis%21USD%2116.80%216.89%21%21%2116.80%216.89%21%402101ea7117283994584186140e1e2f%2166109483839%21sea%21US%214391796073%21X&curPageLogUid=t0X8mgtRuEqd&utparam-url=scene%3Asearch%7Cquery_from%3A) – Any small standoff that fits the Pi’s holes should work fine. I inserted mine into the 3D printed part using a soldering iron. 

---

#### LEDs and Power

- **LEDs and Resistors**:
  - [5mm LEDs](https://shorturl.at/MhEKz) or [alternative link](https://www.aliexpress.us/item/3256805522196114.html?spm=a2g0o.productlist.main.1.73135c11NG8V0z&algo_pvid=3f239b2b-58c5-4eab-986c-39b02707dec4&algo_exp_id=3f239b2b-58c5-4eab-986c-39b02707dec4-0&pdp_npi=4%40dis%21USD%211.68%211.68%21%21%2111.81%2111.81%21%402101ea8c17283982047626731e1e3b%2112000034078716879%21sea%21US%214391796073%21X&curPageLogUid=9dFMfLLQkKbc&utparam-url=scene%3Asearch%7Cquery_from%3A) – Any standard 5mm LED will work; mine were pulled from a DIY Pi kit. 
  - [390 Ohm Resistors](https://shorturl.at/njeu3) or [alternative link](https://www.aliexpress.us/item/3256804747550699.html?spm=a2g0o.productlist.main.3.7977740alkOlOt&algo_pvid=32487002-2eb7-495e-a926-dc5a672d5779&algo_exp_id=32487002-2eb7-495e-a926-dc5a672d5779-1&pdp_npi=4%40dis%21USD%212.31%212.31%21%21%212.31%212.31%21%402101c9ac17283982955918910eccf5%2112000031069410692%21sea%21US%214391796073%21X&curPageLogUid=YZri7EgroMH3&utparam-url=scene%3Asearch%7Cquery_from%3A) – Used for the LEDs. You may want to use a higher resistance as these are quite bright. 
- **Diode**: [3A Diode (supports 5V)](https://a.co/d/aqU21aW) or [alternative link](https://www.amazon.com/dp/B0D4QNTT4V?ref=cm_sw_r_cp_ud_dp_AQAJ49RP5TSYMA0KZTRB_1&ref_=cm_sw_r_cp_ud_dp_AQAJ49RP5TSYMA0KZTRB_1&social_share=cm_sw_r_cp_ud_dp_AQAJ49RP5TSYMA0KZTRB_1&skipTwisterOG=1)
 – This is used to prevent the charging LED from being powered by the battery bank, so it only turns on during charging. This setup prevents the USB-C port from being used as a power source, as noted in the issues section. 
---

#### Cables and Wiring

- **Cables**:
  - [Micro HDMI to HDMI](https://shorturl.at/lDclC) or [alternative link](https://www.aliexpress.us/item/3256802014452724.html?spm=a2g0o.order_list.order_list_main.5.5df11802u5n2FA&gatewayAdapt=glo2usa)
  - [Micro HDMI to Mini HDMI](https://a.co/d/1WwkHYU) or [alternative link](https://www.amazon.com/dp/B08BFZFT7R?ref=cm_sw_r_cp_ud_dp_2QFHWCFVPHJDC0JWJT6R&ref_=cm_sw_r_cp_ud_dp_2QFHWCFVPHJDC0JWJT6R&social_share=cm_sw_r_cp_ud_dp_2QFHWCFVPHJDC0JWJT6R&skipTwisterOG=1)
  - [USB A to USB A](https://shorturl.at/Ay4hM) or [alternative link](https://www.aliexpress.us/item/3256806526879520.html?spm=a2g0o.productlist.main.1.2c1b4851jxyIFD&algo_pvid=b826eab0-3f62-4c1c-94d9-be90fe4566e2&algo_exp_id=b826eab0-3f62-4c1c-94d9-be90fe4566e2-0&pdp_npi=4%40dis%21USD%210.96%210.94%21%21%210.96%210.94%21%402103010f17283990423726422e8976%2112000038073797830%21sea%21US%214391796073%21X&curPageLogUid=jdl8tKrp6YSl&utparam-url=scene%3Asearch%7Cquery_from%3A) – I made my own, but this should work. 
  - [RJ45 Male to RJ45 Male](https://shorturl.at/zojFO) or [alternative link](https://www.aliexpress.us/item/2251832635496878.html?spm=a2g0o.productlist.main.1.2e0ebefaN1aiKa&algo_pvid=2ed1e082-9ba9-4eb1-9e3b-90b305f95d62&algo_exp_id=2ed1e082-9ba9-4eb1-9e3b-90b305f95d62-0&pdp_npi=4%40dis%21USD%211.67%211.67%21%21%211.67%211.67%21%402101effb17283991670993791e80bb%2112000025278965076%21sea%21US%214391796073%21X&curPageLogUid=NhxhG1leGv5l&utparam-url=scene%3Asearch%7Cquery_from%3A)
 – I made my own, but this should work.
- **Wiring and Heatshrink**: I used spare 22AWG wire and heatshrink, but you can find similar materials [here](https://shorturl.at/3O9jX) and [here](https://shorturl.at/ypX5P) for the USB-C and micro USB connections (Pi, screen, and charging). You may need some non-USB-C PD cables and ends to solder up. 
---

#### 3D Printed Parts

- **3D Printed Components**: All parts are printed with [**Polymaker PETG**](https://us.polymaker.com/products/polylite-petg), but any standard filament should work. 
