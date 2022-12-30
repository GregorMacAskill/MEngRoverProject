# Modelling and Control of a Four-Wheeled Rover

Developed by Gregor MacAskill for the University of Glasgow in accordance with the requirements of the degree of Master of Engineering in Aeronautical Engineering in the James Watt School of Engineering.

## Overview of the Project
## Bill of Materials
- M5StickC / M5StickCPlus
- RoverC / RoverC Pro
- Grove 9 DoF IMU or 6 DoF IMU + Magnetometer
## How to Use this Repository
### Commanding Rover
### IMU Data Acquisition
### IMU Data Calibration
### Mahony Filter
### Data Processing
### Video Analysis

## Dependencies and Compatibility
The embedded code within this repository is intended to be used with the M5StickC/M5StickC PLUS and RoverC/RoverC Pro. As such, it relies on the "M5StickC"/"M5StickCPlus" and "M5-RoverC" libraries by M5Stack being installed. These libraries can be downloaded from [M5Stack](https://github.com/m5stack/M5StickC-Plus) directly or via the Arduino IDE. <br />
Since the M5StickC is based on ESP32 microcontroller series, it is recommended to reference the Espressif Systems framework in the 'Additional Board Manager URLs' field in the Arduino IDE as follows with the following link: https://dl.espressif.com/dl/package_esp32_index.json
If the user wishes to utilise remote control of the rover using a PS3 controller via bluetooth, then jvpernis' ["esp32-ps3"](https://github.com/jvpernis/esp32-ps3) library must also be installed.
