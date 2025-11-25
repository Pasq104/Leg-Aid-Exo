# 💻 Software Module — leg-aid-exo

The Software module provides all source code and configuration files required to operate the leg-aid-exo within the OpenExo ecosystem.  
It includes controller implementations, sensor integration, communication interfaces, and utilities for running real-time exoskeleton assistance.

---

## 📁 Contents

- **controller_examples/**  
  Template controllers for hip assistance, torque profiles, gait-phase logic.

- **configuration_files/**  
  Default device settings, joint definitions, and SD-card configurations.

- **utils/**  
  Communication helpers, calibration scripts, and interface functions.

---

## 🧠 Software Architecture

The system follows the OpenExo modular architecture:

- **Teensy 4.1** → high-speed control loop (C++/Arduino)  
- **Arduino Nano BLE 33** → Bluetooth communication  
- **Python API** → GUI control, data collection, parameter tuning

## External Software Documentation
For full details on the control framework and API, refer to:

🔗 https://github.com/naubiomech/OpenExo/tree/main?tab=readme-ov-file

The architecture uses:

- Object-oriented design (inheritance-based polymorphism)  
- Configurable joint setup via SD-card  
- Real-time CAN bus communication with AK-series motors  
- Modular controllers that can be swapped without rewriting the core code  

---

## ⚙️ Controllers

Included controller templates support:

- **Hip torque assistance**  
  Based on gait-phase estimation with FSR sensors.

- **Low-level motor control**  
  PD-based torque tracking, CAN commands.

- **Custom profiles**  
  Users can create their own controller classes by extending the base `Controller` interface.

---

## 🔌 Sensors & I/O

The software supports:

- Force Sensitive Resistors (FSRs)  
- Torque sensors  
- Angle encoders  
- Custom digital/analog inputs  

All sensor usage can be enabled or disabled in the configuration files.

---

## 🔧 Development Workflow

1. Configure device parameters on the SD-card  
2. Build/upload firmware to the Teensy  
3. Connect using the Python GUI  
4. Tune parameters in real time  
5. Log and export data for analysis  

---

## 🤝 Contributions

Contributors can add new controllers, sensor drivers, communication protocols, or improvements to the Python GUI.  
Please follow coding standards and include clear documentation when submitting pull requests.

