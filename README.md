# duckduino

Convert arduino uno in "rubber ducky"

Changes: ready to use at devices with Latin American/Spain distribution

Run: sudo ./script.sh

When guided script indicates, upload /ArduinoUNO_HID/Duckduino/Duckduino.ino file on arduino uno card, changing setup() function by anyone you want

In addition, the script refers to "two pins", these are marked below. You should note that they must be bridged together:

![alt text](https://github.com/cololaborde/duckduino/blob/master/image/image_2022-03-27_00-56-01.png)

Requirements: dfu-programmer

 Debian / Raspbian / Ubuntu /  Kali Linux
 
 apt-get install dfu-programmer
 
 Arch Linux
 
 pacman -S dfu-programmer
 
 Fedora
 
 dnf install dfu-programmer
 
 OS X
 
 brew install dfu-programmer
