# ZigBee IoT Sensor Network with MQTT Integration

This project implements a ZigBee-based IoT sensor network that collects data from various devices (End-Device). The system uses the MQTT protocol for communication between devices and a central ZigBee hub. 

## Features
- **ZigBee Communication**: Collects sensor data from ZigBee-based devices and sends it to a central hub.
- **MQTT Integration**: Uses MQTT protocol for reliable message transmission between the End-Device and the hub.

## Project Setup

### 1. **Hardware Components**:
- ZigBee Hub with CC2652P7 Chip (Coordinator)
- ZigBee End-Device with CC2652P7 Chip
- USB-to-TTL Converter for programming
- Linux-based Hub (with SD card containing the Linux OS)
- Network cable (for internet connection)
  
### 2. **Software Requirements**:
- **MQTT2ZigBee**: Installed on the ZigBee Hub for communication.
- **MobaXterm or Putty**: For SSH communication with the Linux hub.
- **PTVO Software**: For programming the End-Device firmware.

### 3. **Setup Instructions**:

#### A. **Setting up the ZigBee Hub**:
1. Connect the ZigBee Hub to the Linux-based device via USB-to-TTL converter.
2. Use serial communication (e.g., MobaXterm or Putty) to access the hub terminal and set up MQTT2ZigBee.
3. Configure the network and install necessary software (e.g., MQTT2ZigBee firmware) on the hub.

#### B. **Programming the End-Device**:
1. Download PTVO software and create custom firmware for the End-Device (e.g., controlling a sensor like an LED or switch).
2. Use the USB-to-TTL converter to program the End-Device using serial programming methods.
3. Pair the Device-End with the ZigBee Hub using the MQTT2ZigBee configuration.


## Technologies Used:
- **ZigBee** for wireless communication
- **MQTT** protocol for device messaging
- **Linux** for the ZigBee Hub's operating system

