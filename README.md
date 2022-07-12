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
First, the CH559 module must be flashed [See](https://github.com/ScrumPilot616/CH559sdccUSBHost)
Afterward the firmware "USB2RC.ino.esp32.bin" must be uploaded to the ESP32.
Therefore multiple ESP32 firmware uploader tools are available.

An upload is also possible by using the Arduino IDE as described below.

1. Connect ESP32 and PC with an USB-cable
2. Install the latest Arduino IDE
3. Start Arduino IDE
4. In Preferences, Add "https://dl.espressif.com/dl/package_esp32_index.json" to your additional board manager URLs
5. In Preferences, check "Show verbose output during: Upload"
6. In Tools, select "ESP32 Dev Module" as your board
7. In Tools, select the right COM port
8. In File/Examples/ESP32/ChipId select "GetChipID" 
9. Compile and upload the sketch, check the correct upload in serial monitor. ChipID and Model shall be printed.
10. Within the console output, you should see a line like 
    C:\Users\XXXXX\AppData\Local\Arduino15\packages\esp32\tools\esptool_py\3.0.0/esptool.exe --chip esp32 --port COM4 --baud 921600 --before default_reset --after hard_reset write_flash -z --flash_mode dio --flash_freq 80m --flash_size detect 0xe000 C:\Users\XXXXX\AppData\Local\Arduino15\packages\esp32\hardware\esp32\1.0.6/tools/partitions/boot_app0.bin 0x1000 C:\Users\XXXXX\AppData\Local\Arduino15\packages\esp32\hardware\esp32\1.0.6/tools/sdk/bin/bootloader_qio_80m.bin 0x10000 C:\Users\XXXXX\AppData\Local\Temp\arduino_build_404906/GetChipID.ino.bin 0x8000 C:\Users\XXXXX\AppData\Local\Temp\arduino_build_404906/GetChipID.ino.partitions.bin 
11. Create a new batch file like "uploadEsp.bat" and paste the comand line to it.
12. Replace the parameter "C:\Users\XXXXX\AppData\Local\Temp\arduino_build_404906/GetChipID.ino.bin" with the name and the location of your local partition-bin-file e.g. C:\download\USB2RC.ino.bin
12. Replace the parameter "C:\Users\XXXXX\AppData\Local\Temp\arduino_build_404906/GetChipID.ino.partitions.bin" with the name and the location of your local partition-bin-file e.g. C:\download\USB2RC.ino.partitions.bin
13. Start the batch


 


### Configuration Tool
The USB2RC configuration tool "USB2RCConfig.exe" is a part of this repository.

![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RCDataView.png)


### Configuration

1. Connect ESP32 and PC with an USB-cable
2. Start USB2RCConfig.exe on the PC
3. Select the correct COM-Port
4. Press the <Connect>-button
5. Press the <Configuration>-Button
6. Configure the box to your belongings
7. Press the <Save>-Button

![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RCConfiguration.png)

### License Key
Even if you have to upload a valid license key, this software is for free.
You can request a licence key by pushing a request with your device ID to the 
discussion. To visualize the device ID or to upload the licence key press the <Licence>-Button.
The device ID is only shown if no valid license key is available.

![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RCLicense.png)




## Used Libraries

| Library     | Author | Licence |
| ----------- | ------ | ------- |
| esp8266-oled-ssd1306 | Copyright (c) 2016 by Daniel Eichhorn,Fabrice Weinberg | MIT |



## Example builds
### Build by ScrumPilot616

Front
![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RC_SP_Example1.png)

Back
![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RC_SP_Example2.png)

Oled
![N|Solid](https://github.com/ScrumPilot616/USB2RC/blob/main/images/USB2RC_SP_Example3.png)




