# duckduino

Convert arduino uno in "rubber ducky"

Forked from: https://github.com/Lacerda53/duckduino  

Changes: ready to use at devices with Latin American/Spain keyboard distribution

## Instructions

```bash
sudo ./script.sh
```

When guided script indicates, upload /ArduinoUNO_HID/Duckduino/Duckduino.ino file on arduino uno card, changing setup() function by anyone you want

In addition, the script refers to "two pins", these are marked below. You should note that they must be bridged together:

![alt text](https://github.com/cololaborde/duckduino/blob/master/image/image_2022-03-27_00-56-01.png)

## Requirements: dfu-programmer

 ### Debian / Raspbian / Ubuntu /  Kali Linux
 ```bash
 apt-get install dfu-programmer
 ```

 ### Arch Linux
 
 ```bash
 pacman -S dfu-programmer
 ```
 
 ### Fedora
 ```bash
 dnf install dfu-programmer
 ```
 ### OS X

 ```bash
 brew install dfu-programmer
 ```


## Firmware Factory Reset:

```bash
sudo dfu-programmer atmega16u2 erase

sudo dfu-programmer atmega16u2 flash Arduino-usbserial-uno.hex

sudo dfu-programmer atmega16u2 reset
```