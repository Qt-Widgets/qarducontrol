QArduControl
============

## Details ##
Burn once and control your Arduino board via USB/Serial.

## Features ##
* Turn on/off digital pins
* Write values (0-255) to PWM pins
* Read analog input pins (0-1023)
* Read uptime in millis

## Requirements ##
* Qt 4/5
* QtSerialPort library
* Arduino Uno board/other compatible boards

## How to use ##
You need to burn `sketch/QArduControl.ino` to your MCU and then connect it via usb/serial port.

## Installing QtSerialPort ##
If you don't have Qt5, then QtSerialPort is available for download at from its gitorious repository.

```
git clone git://gitorious.org/qt/qtserialport.git
```
After cloning, cd to it and build.
```
cd qtserialport
qmake
make
sudo make install
```
## Screenshots ##
QArduControl GUI

![QArduControl GUI](http://i.imgur.com/nrHe50M.png "QArduControl GUI")

Software Reset Menu

![Software Reset Menu](http://i.imgur.com/rOCJIm0.png "Software Reset Menu")

## TODO/FIXME ##
* Fix digital write conflict
* Add save pin state on software reopen
