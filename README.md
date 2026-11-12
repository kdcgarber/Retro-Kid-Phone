![](images/trs-80MotherboardKeyBoard3.jpg?raw=true)


<h1>
  <img src="images/Side.jpg" width="100" height="150" align="right" alt="Retro Kid Phone">
  Retro Kid Phone
</h1>
<br>


These are my notes:

This is a retro-inspired phone case built for the open-source Kid-Phone firmware project which is designed around an ESP32-S3 and Twilio phone service. 
This repository contains the custom 3D printable enclosure, wiring references, assembly photos, and a few build notes used to create a fully functional WiFi Kid-Phone enclosure.

---

## Overview

While searching for WIFI phones for the grandkids that would use a microcontroller, <br>
I discovered this interesting ESP32 projects by Allan Binder. <br>
The concept is excellent, but I wanted a more retro-inspired enclosure that looked like a classic desktop telephone for the grandkids.

This project combines the original Kid-Phone software, which is an amazing project, and my custom-designed 3D printed enclosure with the illuminated arcade-style pushbuttons.

### Original Project Resources

**Project Article**
https://muonsortes.com/toddler-phone#using <br>
**GitHub Repository**
https://github.com/AllanBinder/kid-phone <br>
**Web Installer**
https://allanbinder.github.io/kid-phone/ <br>

---

## Features
- Retro telephone inspired enclosure that is fully 3D printable
- Kid-phone:
	- ESP32-S3 based design
	- Large illuminated pushbuttons
	- Easy firmware installation using the official web installer
	- Local web-based configuration interface


---

## Repository Contents

```text
.
├── 3d
│   ├── retroPhoneKid-phone-Bottom.stl
│   ├── retroPhoneKid-phone-SPI32Cover.stl
│   ├── retroPhoneKid-phone-Top.stl
│   └── retroPhoneKid-phone.3mf
└── images
```

### Included Files

| File | Description |
|--------|-------------|
| retroPhoneKid-phone-Bottom.stl | Phone bottom housing |
| retroPhoneKid-phone-SPI32Cover.stl | ESP32-S3 cover |
| retroPhoneKid-phone-Top.stl | Phone top housing |
| retroPhoneKid-phone.3mf | All components arranged for printing |
<br>
The included 3MF file contains all parts pre-positioned for printing.
<br>
---

# Design Gallery

## Front View
These are pictures of the Phone when assembled and running with the buttons illuminated

| CAD Design | Printed Assembly |
|------------|------------------|
| <img src="images/FrontDrawing.jpg" width="700" height="600"> | <img src="images/TopOfPhone.jpg" width="700" height="600"> |

---

## Back View
Clear labeling on the back indicates the USB handset and USB power locations. 

| CAD Design | Printed Assembly |
|------------|------------------|
| <img src="images/BackDrawing.jpg" width="700" height="600"> | <img src="images/BackOfPhone.jpg" width="700" height="600"> |

---

## Bottom View
The ESP32 status lights are viewable through the bottom plate.
<img src="images/Bottom.jpg" width="500" height="600">

---

## ESP32 Wiring Reference

| GPIO Wiring | Placement |
|-------------|-------------------|
| <img src="images/esp1.jpg" width="700" height="600"> | <img src="images/esp2.jpg" width="700" height="600"> |

---

## Wiring Reference

| GPIO Wiring | Connection Diagram |
|-------------|-------------------|
| <img src="images/GPIOToWires.png" width="700" height="600"> | <img src="images/WireConnections.png" width="700" height="600"> |

---


## Internal Assembly

I used the chart above to add wires to each of the GPIO’s on the ESP32. <br>

Adding 2 sets of 4 wires: <br>
 Button - RED/GREEN/BLUE/YELLOW <br>
 LED - RED/GREEN/BLUE/YELLOW <br>
 GND - BLACK. <br>

The connection diagram shows a color-coded dot next to the ESP32 locations that I solder wires on to. <br>
I then separated the LED wires and the button wires each on their own side of the <br> enclosure, then closed the ESP32 cover. <br>
I next soldered all the ground (GND) wires to the - on the leds <br>
and one pin of the switch as seen in the zoomed in picture below. <br>
I then solder the remaining 8 exposed wires to the correct light and switch. <br>
Match each wire color to the button color for ease and clarity. <br>
The wires that show on the right from the bottom are the ones that connect to the LED pins. <br>
The wires on the left connect to the switches. <br>
When complete, I used 4 -M3*8 flat head screws to join the bottom and the the top together. <br>

<img src="images/InsidePhone.jpg" width="600" height="700">
<img src="images/ButtonWires.jpg" width="700" height="600">
---

# Firmware Installation

Install the Kid Phone firmware using the official installer:

https://allanbinder.github.io/kid-phone/

Follow the instructions provided by the original project documentation.

---

# Device Configuration

After connecting the Kid Phone to WiFi, configuration can be accessed using:

http://kidphone.local/

---

# Bill of Materials

## ESP32-S3 Development Board

Purchase Link: https://www.amazon.com/dp/B0CKXJLP4B

<img src="images/ESP32-S3.png" width="700" height="600">)

( You really only need one, but I bought a set of three for other projects)

---

## Illuminated Pushbuttons

Purchase Link: https://www.amazon.com/dp/B07L3XF6V9

| Product Listing | Installed In Project |
|----------------|---------------------|
| <img src="images/ButtonsAmazon.png" width="700" height="600"> | <img src="images/BottonsUsed.jpg" width="700" height="600"> |

---


## Handset

Purchase Link:  https://www.amazon.com/dp/B0HKHJDL5S

<img src="images/Handset.png" width="700" height="600"> 
(This is the link to the handset I ordered, it seems to work well, <br>
though the buttons on the handset are not the same configuration as the Amazon picture shows.) <br>

---


# Printing Notes

- Print all enclosure components using the supplied STL files or better yet, 
  use the included 3MF file that provides the recommended orientation for a cleaner print.

---

# Credits

This enclosure design was created for use for the Kid-Phone project.

Special thanks to:

- Allan Binder
- The Kid Phone project contributors
