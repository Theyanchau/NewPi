## Raspberry Pi 4 101

### How to run a PI?
You will need :

* Raspberry Pi
* Network cable(connect PI directly to from PC)
* Display cable(micro hdmi cable)
* Power cable (Type C)
* Micro SD card (Storing Pi OS)

---

# Installing Pi OS
The Pi itself doesn't contain any OS software, you will need to install Pi OS in the Micro SD card and insert to your Pi.
There are 2 ways to Install Pi OS:
1. Install Pi OS using Raspberry Pi Imager 
2. Manually install an operating system image


## Raspberry Pi Imager
Raspberry Pi Imager is a quick and easy tool to install Raspberry Pi OS and other operating systems to a microSD card. 

[Download Paspberry Pi Imager](https://www.raspberrypi.org/software/)



## Manually Install 
You could download the operating system directly from Pi offical website.

[Downlaod operating system](https://www.raspberrypi.org/software/operating-systems/)


# Errors

## Error writing to storage when using Raspberry Pi Imager
What cause? Raspberry Pi OS doesn't work on **exFAT** format, you will need to change your SD card to **FAT32** partition. 

1. Check your SD card format

### How can you check your SD card format?
1. Open file explorer
2. Right click on SD card and Choose "Properties"
3. In the Properties, look for File system. The term next to File system is your SD card format


## What is exFAT?
exFAT is a file system that is typically found on SD cards and USB flash drives. It has been optimized for flash memory like these. For SDXC cards over 32 GB it is the default filesystem. It supports larger files than FAT32 but has less overhead than NTFS.

Supported by many newer versions of systems (Windows, OSX, Linux, Cameras, etc.)
16 exbibyte file size limit
great for SD cards, USB drives, and cameras
easy to implement in firmware ( on cameras )
