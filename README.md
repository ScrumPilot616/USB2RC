# USB2RC


## Features
- Two USB input devices
- 12 channel CPPM output
- 16 channel CRSF output
- Headtracker serial input
- WiFi/Bluetooth telemetry output

## Supported USB Dvices
- T-Flight Hotas X, PC and PS3 mode

Further devices will follow.

## Hardware


### Required
- ESP32
- CH559 USB-Host

### Optional
- OLED SSD1306 
- Voltage divider
- Passive buzzer
- LAB USB2RC Board
 
### Wiring
You can build the circuit by your own or order the USB2RC board at LAB (Link will follow)

![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RCWiring.png)


## Installation

### Flashing Firmware
#### CH559 Module
The CH559 module must be flashed with the following firmware: [CH559sdccUSBHost](https://github.com/ScrumPilot616/CH559sdccUSBHost)


#### ESP32
Download the "Flash Download Tools" from the Expressif homepage.
Start the tool and set the following properties:

![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/ESP32Flashing.png)

Presss the "Start"-Button

 


### Configuration Tool
The USB2RC configuration tool "USB2RCConfig.exe" is a part of this repository.

![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RCDataView.png)


### Configuration

1. Connect ESP32 and PC with an USB-cable
2. Start USB2RCConfig.exe on the PC
3. Select the correct COM-Port
4. Press the "Connect"-Button
5. Press the "Configuration"-Button
6. Configure the box to your belongings
7. Press the "Save"-Button

![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RCConfiguration.png)

### Activation key
Even if you have to upload a valid activation key, this software is for free.
You can request a activation key by pushing a request with your device ID to the 
[discussion](https://github.com/ScrumPilot616/USB2RC/discussions/categories/activation-key-requests) of this repository .
To visualize the device ID or to upload the activation key press the "Activation"-Button.
The device ID is only shown if no valid activation key is available.

![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RCActivation.png)




## Used Libraries

| Library     | Version | Licence |
| ----------- | ------ | ------- |
| [ESP8266 and ESP32 OLED driver for SSD1306 displays](https://github.com/ThingPulse/esp8266-oled-ssd1306)| 4.3.0 | MIT |
| [Arduino core for the ESP32](https://github.com/espressif/arduino-esp32) | 1.0.6 |  LGPL-2.1   |

For detailed license information see [COPYING.md](./COPYING.md)




## Example builds
### Build by ScrumPilot616

Front
![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RC_SP_Example1.jpg)

Back
![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RC_SP_Example2.jpg)

Oled
![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RC_SP_Example3.jpg)




