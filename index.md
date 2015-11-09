---
layout: default
title: Home
---

# This Document
***
This is a quick and simple tutorial to provide some basic knowledge and links to other references about the Raspberry Pi.

# Beginnings
***
This part will show you how to install the Raspbian Linux image onto your Raspberry Pi.

## \# Requirements
- Raspberry Pi 2 (model B)
- Micro-USB power connector (similar to ones plugged into most Android phones)
- Micro SD Card (at least 4Gb)
- Micro SD Card reader (to read/flash the SD card)
- Connectivity to Pi [Display](#display)

## \# Directions
Go to the installation page that the Raspberry Pi Foundation provides [here](https://www.raspberrypi.org/documentation/installation/installing-images/README.md).

Choose your respective operating system of choice for flashing the SD card on the installation page. The instructions there are nearly perfect and even have some troubleshooting tips.

# Extras
***
A list of extra items and helpful topics

## \# Display
One of the *features* of the Raspberry Pi is that it is a headless system and can function without a monitor, provided another means of connection is available. I will demonstrate two common methods of connection:

### 1. HDMI with Monitor w/Keyboard and Mouse
Plugging in an HDMI cable into the Pi while it is turned on will provide a GUI interfaced display to interact with. This is typical to a normal computer interface and will act as such, the only issue that it has a small processor and rendering the screen cause lag on inputs.

### 2. SSH with Ethernet Connection
When the Pi is plugged into a router with the Ethernet port, it can be accessed with SSH. Typical Linux/Unix platforms provide SSH access from terminal but Windows can achieve SSH access with [PuTTY](http://www.chiark.greenend.org.uk/~sgtatham/putty/).

One of the noted issues with this configuration is that the IP address of the Raspberry Pi must be known in order to connect to it via SSH. Either static IP or router access must be needed in order to connect with the Raspberry Pi through SSH.

# Links
***
- [Raspberry Pi](https://www.raspberrypi.org/)
- [Raspbian Download](https://www.raspberrypi.org/downloads/raspbian/)
