# USB2RC


## Features
- PPM output
- CRSF output
- Headtracker serial input
- WiFi telemetry output

## Hardware

### Required
- ESP32
- CH559 USB-Host [See](https://github.com/ScrumPilot616/CH559sdccUSBHost)

### Optional
- OLED SSD1306 
- Voltage devider for measuring box supply 
- Passive buzzer
- LAB USB2RC Board
 
### Wiring
You can build the circuit by your own or order the USB2RC board at LAB (Link will follow)

![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RCWiring.png)


## Installation

### Flashing Firmware
#### CH559 Module
First, the CH559 module must be flashed [See](https://github.com/ScrumPilot616/CH559sdccUSBHost)


#### ESP32
First, download the "Flash Download Tools" from the Expressif homepage.
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

### License Key
Even if you have to upload a valid license key, this software is for free.
You can request a licence key by pushing a request with your device ID to the 
discussion. To visualize the device ID or to upload the licence key press the <Licence>-Button.
The device ID is only shown if no valid license key is available.

![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RCLicense.png)




## Used Libraries

| Library     | Version | Licence |
| ----------- | ------ | ------- |
| esp8266-oled-ssd1306 |  | MIT |
| Arduino core for the ESP32 | 1.0.6 |  LGPL-2.1 license  |




## Example builds
### Build by ScrumPilot616

Front
![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RC_SP_Example1.jpg)

Back
![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RC_SP_Example2.jpg)

Oled
![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RC_SP_Example3.jpg)




