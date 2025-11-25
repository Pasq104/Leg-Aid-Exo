# 🔌 Electronics Module — leg-aid-exo

The Electronics module contains all electrical design resources required to operate the leg-aid-exo exoskeleton.  
This subsystem includes PCB interfaces, wiring diagrams, sensor integrations, motor communication setups, and firmware utilities based on the OpenExo electrical architecture.

---

## 📁 Contents

- **wiring/**  
  Connection diagrams for actuators, sensors, power distribution, and microcontrollers.

- **pcb/**  
  PCB schematics, pinouts, fabrication files, and interface notes for the OpenExo board.

- **firmware/**  
  Low-level configuration helpers, CAN communication examples, calibration scripts, and microcontroller setup files.

---

## ⚡ System Architecture

The electronics follow the standard OpenExo hardware structure, designed for modularity and easy replication:

- **Teensy 4.1**  
  High-speed control, sensor acquisition, and CAN motor communication.

- **Arduino Nano BLE 33**  
  Handles Bluetooth Low Energy (BLE) communication with the Python GUI.

- **OpenExo PCB**  
  Custom board enabling power distribution, sensor conditioning, and motor connectivity for up to two joints simultaneously.

This system allows rapid swapping of actuators (AK60, AK70, AK80 series), sensors, and joint configurations without rewriting core electronics.

---

## 🔧 Supported Actuators & Sensors

### **Actuators**
- CubeMars AK-series motors  
  - AK60-6 v1.1  
  - AK70-10  
  - AK80-9  
- Communication protocol: **CAN Bus**

### **Sensors**
- Force Sensitive Resistors (FSRs)  
- Torque sensors  
- Magnetic angle encoders  
- Optional custom analog or digital sensors

All sensors can be enabled/disabled via configuration files in the software module.

---

## 🔋 Power & Safety

- Compatible with Li-Ion 22.2V battery packs  
- Built-in overcurrent and undervoltage protection  
- Motor temperature monitoring supported  
- Documentation includes safe operating ranges and connection guidelines

---

## 🔗 Integration With Software

The electronics module interfaces directly with the Software subsystem:

- CAN communication handled by Teensy  
- Parameter updates and data streaming handled via BLE (Nano 33)  
- SD-card configuration loads default settings for joint and sensor setup  

Firmware examples in the `firmware/` folder demonstrate motor initialization, sensor reading, and control loop communication.

---

## 📚 Documentation

Reference documents:

- Wiring diagrams  
- PCB assembly instructions  
- Connector pinouts  
- Sensor calibration notes  
- Motor setup guides  

These resources ensure a smooth assembly process and simplify troubleshooting.

---

## 🤝 Contributions

Electrical improvements, PCB optimizations, and additional sensor integrations are welcome.  
Please include schematics, Gerber files, and testing notes when contributing new hardware revisions.

