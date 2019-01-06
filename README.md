# Build a Raspberry Pi Ethical Hacking Computer
In this training lab you will learn how to set up an ethical hacking computer using the Raspberry Pi.
(wow readers with raspberry pi facts/stats)
The affordability of the Raspberry Pi and its stealthy size makes it a perfect testing device.
(INTRO TO KALI)
For our operating system we'll be using Kali Linux. If you are not familiar with Kali Linux, you should know that it is an advanced penetration testing and network security assessment tool.

## Supplies
- [Raspberry Pi 3 B+ Motherboard](https://www.amazon.com/ELEMENT-Element14-Raspberry-Pi-Motherboard/dp/B07BDR5PDW/ref=sr_1_3?ie=UTF8&qid=1541551736&sr=8-3&keywords=raspberry+pi+3+b%2B)
- [16GB micro SD card](https://www.amazon.com/Sandisk-Ultra-Micro-UHS-I-Adapter/dp/B073K14CVB/ref=sr_1_2?s=electronics&ie=UTF8&qid=1541551914&sr=1-2&keywords=sandisk+16gb+micro+sd) (32GB recommended)
- [Wireless Keyboard with Mouse Touchpad](https://www.amazon.com/Rii-Wireless-Keyboard-Touchpad-Control/dp/B00I5SW8MC/ref=sr_1_1?s=electronics&ie=UTF8&qid=1541552109&sr=1-1&keywords=Rii+Mini+Wireless+2.4GHz+Keyboard+with+Mouse+Touchpad+Remote+Control%2C+Black+%28mini+X1%29)
- [Case with fan, power supply](https://www.amazon.com/Smraza-Raspberry-Heatsinks-Supply-Compatible/dp/B07GKXZH7X/ref=sr_1_32?ie=UTF8&qid=1541552913&sr=8-32&keywords=Smraza#customerReviews)

The [CanaKit Raspberry Pi 3 B+](https://www.amazon.com/CanaKit-Raspberry-Premium-Clear-Supply/dp/B07BC7BMHY/ref=sr_1_1?s=pc&ie=UTF8&qid=1541553553&sr=1-1&keywords=CanaKit+Raspberry+Pi+3+B%2B+%28B+Plus%29+with+Premium+Clear+Case+and+2.5A+Power+Supply) bundle is a good starter kit as well.

Supported models for this build:
- Raspberry Pi 3  B+
- Raspberry Pi 3 B
- Raspberry Pi 2
- Raspberry Pi Zero W

## Instructions

### Step 1: Download Kali Linux
Download the Kali Linux ARM image for Raspberry Pi [here](https://www.offensive-security.com/kali-linux-arm-images/).

Download Kali Linux image from the Re4son's kernel [here](https://whitedome.com.au/re4son/sticky-fingers-kali-pi-pre-installed-image/).

For extra security, verify the download. This step is optional, but wise to consider if you're downloading the Kali Linux image over a network other than your own.

### Step 2: Flash Kali Linux Image
Format micro SD card before use with [SD Memory Card Formatter](https://www.sdcard.org/downloads/formatter_4/index.html).

**Windows**
Use [Win32 Disk Imager](https://sourceforge.net/projects/win32diskimager/) to write the Kali Linux image to the micro SD card.

**Mac**
Use [Etcher](https://www.balena.io/etcher/) to write the Kali Linux image to the micro SD card.

### Step 3: Boot into Kali Linux
Default credentials for logging in are Username: `root` Password: `toor`

A welcome panel will appear after login. Select "Use default config" (picture of screen saved on iPhone)

### Step 4: Change the default password
Go to terminal, type

```shell
$ passwd root
```

### Step 5: Update & Upgrade
This step requires an internet connection.

### Step 6: Resize Partition
Two ways to do this: via terminal or graphical user interface.

### Step 7: Change hostname
nano /etc/hostname
In this example we'll use "Kali_Pi"
Press CTRL + X to exit. You will then be prompted to save your changes. Press Y to save.
Press Enter to confirm the file name the changes will be applied to.

nano /etc/hosts
Change "kali" to "Kali_Pi"
CTRL+X, Y, Enter

Reboot. We should now see the hostname changed in our terminal prompt.

### Step 8: Setup SSH
Verify whether the SSH service is installed:

service --status-all

### Step 9: Change the Default SSH keys

### Step 10: Reverse Shell Through SSH

### Enable Auto Login with SSH
https://www.novaspirit.com/2018/04/24/kali-linux-raspberry-pi-3b-monitor-mode/

### Enable Bluetooth


**Resources:**
https://gbhackers.com/raspberry-pi-and-kali-linux/
https://blog.underc0de.org/instalar-kali-en-raspberri-pi/

- prevent Kali Linux from sleeping
- Disable screen lock

Things to do after installing Kali Linux:
- https://null-byte.wonderhowto.com/how-to/top-9-things-do-after-installing-kali-linux-0186450/
