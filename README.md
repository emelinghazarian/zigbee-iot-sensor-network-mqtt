# ZigBee IoT Sensor Network with MQTT Integration and Web Dashboard

This project implements a ZigBee-based IoT sensor network that collects data from various devices (Device-End) and displays it on a web dashboard. The system uses the MQTT protocol for communication between devices and a central ZigBee hub. 

## Features
- **ZigBee Communication**: Collects sensor data from ZigBee-based devices and sends it to a central hub.
- **MQTT Integration**: Uses MQTT protocol for reliable message transmission between the Device-End and the hub.
- **Web Dashboard**: Provides real-time monitoring and control of devices via a web-based interface.

## Project Setup

### 1. **Hardware Components**:
- ZigBee Hub with 7P2652CC Chip (Coordinator)
- ZigBee Device-End with 7P2652CC Chip
- USB-to-TTL Converter for programming
- Linux-based Hub (with SD card containing the Linux OS)
- Network cable (for internet connection)
  
### 2. **Software Requirements**:
- **MQTT2ZigBee**: Installed on the ZigBee Hub for communication.
- **MobaXterm or Putty**: For SSH communication with the Linux hub.
- **PTVO Software**: For programming the Device-End firmware.

### 3. **Setup Instructions**:

#### A. **Setting up the ZigBee Hub**:
1. Connect the ZigBee Hub to the Linux-based device via USB-to-TTL converter.
2. Use serial communication (e.g., MobaXterm or Putty) to access the hub terminal and set up MQTT2ZigBee.
3. Configure the network and install necessary software (e.g., MQTT2ZigBee firmware) on the hub.

#### B. **Programming the Device-End**:
1. Download PTVO software and create custom firmware for the Device-End (e.g., controlling a sensor like an LED or switch).
2. Use the USB-to-TTL converter to program the Device-End using serial programming methods.
3. Pair the Device-End with the ZigBee Hub using the MQTT2ZigBee configuration.

#### C. **Setting up the Web Dashboard**:
1. Deploy the web-based dashboard on the Linux Hub.
2. Use MQTT protocol to link the dashboard with the ZigBee Hub for real-time device control and monitoring.
3. Access the dashboard via a web browser on your computer or mobile device.

## Technologies Used:
- **ZigBee** for wireless communication
- **MQTT** protocol for device messaging
- **Linux** for the ZigBee Hub's operating system
- **Web technologies** for dashboard display (e.g., HTML, JavaScript)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- Special thanks to the MQTT2ZigBee community for providing the necessary software and documentation.
- Thanks to PTVO for offering a platform to develop custom firmware for ZigBee devices.
