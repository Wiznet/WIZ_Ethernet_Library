WIZ Ethernet Library
========
The Ethernet library lets you connect to the Internet or a local network.  

## Supported devices
* ioShield, WIZ550io (using W5500)
* W5200 Ethernet Shield, WIZ820io (using W5200)
* Arduino Ethernet Shield (using W5100)

## Hardware
* ioShield  
* [W5200 Ethernet Shield](https://github.com/Wiznet/W5200-Ethernet-Shield "W5200 Ethernet Shield")  
* [Ethernet Shield](http://arduino.cc/en/Main/ArduinoEthernetShield "Ethernet Shield")  

## Software
#### Install WIZ Ethernet library  
Download all files and overwrite onto the"Arduino\libraries\Ethernet" folder in your project in sketch.

#### Select device(shield)  
Uncomment the device(shield) you want to use.  
```cpp
//Arduino\libraries\Ethernet\utility\w5100.h
#ifndef	W5100_H_INCLUDED
#define	W5100_H_INCLUDED

#include <avr/pgmspace.h>
#include <SPI.h>

typedef uint8_t SOCKET;
//#define W5100_ETHERNET_SHIELD
//#define W5200_ETHERNET_SHIELD
#define W5500_ETHERNET_SHIELD
```
## How to use the WIZ Ethernet library and evaluate existing Ethernet example.
All other steps are the same as the steps from the Arduino Ethernet Shield. You can find examples in the Arduino IDE, go to Files->Examples->Ethernet, open any example, then copy it to your sketch file (gr_sketch.cpp) and change configuration values properly.
After that, you can check if it is work well. For example, if you choose 'WebServer', you should change IP Address first and compile and download it. Then you can access web server page through your web browser of your PC or something.

## Revision History
* Initial Release : 14 August 2013
* Adding function to read / write W5500 PHY configuration register : 4 December 2013