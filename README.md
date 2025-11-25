# 🦿 leg-aid-exo  
*A modular lower-limb assistive exoskeleton built on the OpenExo open-source framework*

---

## 📘 Overview

**leg-aid-exo** is an open-source project designed to provide a lightweight, modular, and accessible lower-limb assistive exoskeleton.  
The system is based on the OpenExo architecture and aims to support research, prototyping, education, and early-stage development of wearable robotics.

The repository is structured into mechanical, electrical, software, and documentation sections, allowing different development groups to work independently while maintaining a unified ecosystem.

---

## 🛠️ Project Structure

```
leg-aid-exo/
│
├── hardware/         → Mechanical components (CAD, 3D print files, uprights, cuffs)
├── electronics/      → PCB, wiring diagrams, sensors, motor interfaces
├── software/         → Controller logic, configuration files, utilities
├── guida/            → PDF guides and official OpenExo documentation
│
├── README.md         → Main documentation (this file)
└── LICENSE           → Project license
```

---

## ⚙️ Mechanical Module

The mechanical system includes:

- 3D-printable components  
- Carbon-fiber and CNC machined parts  
- Adjustable thigh cuffs  
- Motor mounting brackets  
- Assembly instructions and sizing documentation  

Designed to be lightweight, modular, and easy to reproduce or customize.

---

## 🔌 Electronics Module

The electronics subsystem contains:

- Wiring diagrams and connector layouts  
- OpenExo PCB references  
- Teensy 4.1 + Arduino Nano BLE 33 microcontroller integration  
- CAN bus communication for AK-series actuators  
- Sensor mapping (FSRs, torque sensors, angle encoders)  

Built for easy modification and compatibility with the OpenExo framework.

---

## 💻 Software Module

The software module provides:

- Controller templates (hip torque assistance, gait-phase estimation)  
- SD-card configuration files  
- Sensor calibration utilities  
- Communication helpers for CAN and BLE  
- Support for the Python GUI used for real-time monitoring and tuning  

Modular architecture allows easy integration of new controllers and sensors.

---

## 📘 Documentation (`guida/`)

This folder contains:

- PDF build guides  
- Material lists  
- Assembly diagrams  
- Official OpenExo documentation  

All documents remain under their original licenses (e.g., CC BY-ND 4.0).

---

## 📚 Related Software Documentation

The leg-aid-exo project builds upon the OpenExo software ecosystem.  
Full documentation, source code, and technical details for the control framework can be found here:

🔗 https://github.com/OpenExoProject/OpenExo

---

## 📄 Licensing Notice

All OpenExo PDF documents included in this repository retain their original copyright and are redistributed under their respective open-source licenses (e.g., CC BY-ND 4.0).  
No modifications have been made to the original files.

---

## 🤝 Contributions

Contributions are welcome!  
Mechanical, electronics, and software improvements can be submitted through pull requests.  
Please document any new components or features clearly and maintain consistency with the project structure.

---

## 🌐 Acknowledgements

This project uses open-source materials and documentation from the OpenExo ecosystem.  
Special thanks to the authors and contributors of the OpenExo framework for enabling open research in wearable robotics.

