# Modelling and Control of a Four-Wheeled Rover

Developed by Gregor MacAskill for the University of Glasgow in accordance with the requirements of the degree of Master of Engineering in Aeronautical Engineering in the James Watt School of Engineering.

## Overview of the Project
The objectives of this project are as follows:
- To develop a six degrees-of-freedom mathematical model of a rover with four mecanum wheels.
- To experimentally validate a simplified three degree-of-freedom portion of this model.
- To design and test a suitable control system for the rover using the validated simulation.
- To implement this control system on physical rover hardware and assess its performance.

<!-- END LIST -->

In the process of achieving these objectives, code has been generated to carry out a wide range of processes. All of the code needed to replicate the tests and results of this project are available in this repository and are described below.


## Bill of Materials
Below is a list of required components to fully utilise the functionality of this library:
- M5StickC / M5StickCPlus
- RoverC / RoverC Pro
- Grove 9 DoF IMU or 6 DoF IMU + Magnetometer 

<!-- END LIST -->

Note that any hardware continaing a combination of accelerometer, gyroscope, and magentometer (be it standalone or integrated) is acceptable, however, the sensor data retrieval code may need to be altered to accomodate different hardware. For this project, a [Grove - IMU 9 DoF v2.0](https://wiki.seeedstudio.com/Grove-IMU_9DOF_v2.0/) from Seeed Studio was used.

## Contents of this Repository
### Commanding Rover
### IMU Data Acquisition
### IMU Data Calibration
### Mahony Filter
### Data Processing
### Video Analysis

## Dependencies and Compatibility
The embedded code within this repository is intended to be used with the M5StickC/M5StickC PLUS and RoverC/RoverC Pro. As such, it relies on the "M5StickC"/"M5StickCPlus" and "M5-RoverC" libraries by M5Stack being installed. These libraries can be downloaded from [M5Stack](https://github.com/m5stack/M5StickC-Plus) directly or via the Arduino IDE. <br /> <br />
Since the M5StickC is based on ESP32 microcontroller series, it is recommended to reference the Espressif Systems framework in the 'Additional Board Manager URLs' field in the Arduino IDE with the following link: https://dl.espressif.com/dl/package_esp32_index.json .<br /> 
This will make the "ESP32 Dev Module" an option within the board manager section of the Arduino IDE. <br /> <br />
If the user wishes to utilise remote control of the rover using a PS3 controller via bluetooth, then jvpernis' ["esp32-ps3"](https://github.com/jvpernis/esp32-ps3) library must also be installed.
