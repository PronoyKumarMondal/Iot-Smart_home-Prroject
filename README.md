
# Arduino Projects: Door Control System & LPG-Flame Detection

Welcome to the repository for my Arduino projects! This repository contains two essential projects for home automation and safety: a **Door Control System with Temperature Monitoring** and an **LPG & Flame Detection System**.

## Table of Contents

- [About](#about)  
- [Features](#features)  
- [Technologies Used](#technologies-used)  
- [Projects](#projects)  
- [Circuit Connections](#circuit-connections)  
- [Setup Instructions](#setup-instructions)  
- [How to Upload Code](#how-to-upload-code)  

---

## About

This repository contains Arduino-based projects designed to improve safety and automation in homes.  

1. **Door Control System**: A smart system featuring a keypad, LCD display, motion detection, and remote control via WiFi.  
2. **LPG & Flame Detection System**: Enhances safety by detecting gas leaks and fire hazards, triggering alarms and a water pump.  

---

## Features

### Door Control System  
- **Password-Protected Door Lock**: Uses a servo motor to secure or unlock the door.  
- **Temperature Monitoring**: Displays real-time temperature on an LCD screen.  
- **Motion Detection**: Detects movement for additional security.  
- **WiFi Control**: Operated remotely using the RemoteXY app.
- **[Door Control System Simulation Link](https://wokwi.com/projects/416190208386689025)**
<img src="https://github.com/user-attachments/assets/b44dc2ca-e726-4ceb-9737-aa8ced78e630" alt="Door Control System" width="600px">

### LPG & Flame Detection System  
- **LPG Leak Detection**: Triggers an alarm for high gas concentration.  
- **Flame Detection**: Activates a water pump and buzzer when a flame is detected.  

---

## Technologies Used

- **Hardware Components**:  
  - Arduino UNO  
  - Keypad (4x4)  
  - LCD (I2C)  
  - Servo Motors  
  - Flame Sensor  
  - LPG Gas Sensor  
  - Temperature Sensor  
  - Motion Sensor  
  - Buzzer  
  - Water Pump  
  - WiFi Module (ESP8266)  

- **Software Tools**:  
  - Arduino IDE for coding and sketch uploading.  
  - RemoteXY for mobile app control.  
  - Libraries:  
    - `Servo`  
    - `Keypad`  
    - `LiquidCrystal_I2C`  
    - `RemoteXY`  

---

## Projects

### 1. **Door Control System**  
Combines security and automation into a single system for smart home applications.  

- **Servo-Based Door Lock**: Opens or closes based on the correct password entered via the keypad.  
- **Temperature Monitoring**: Displays live temperature data on the LCD.  
- **Remote Control**: Operated wirelessly via the RemoteXY app.
  
  <img src="https://github.com/user-attachments/assets/0590e0ae-2f38-4b80-b86b-34a1062f01a4" alt="Door Control System" width="600px">

### 2. **LPG & Flame Detection System**  
Focuses on detecting hazards to ensure home safety.  

- **LPG Detection**: Sounds an alarm if gas concentration exceeds a safe level.  
- **Flame Detection**: Activates the water pump and buzzer when a fire is detected.  

---

## Circuit Connections

### Door Control System

#### Keypad Connections
| Keypad Pin | Arduino Pin |
|------------|-------------|
| Row 1      | Pin 13      |
| Row 2      | Pin 12      |
| Row 3      | Pin 11      |
| Row 4      | Pin 10      |
| Col 1      | Pin 9       |
| Col 2      | Pin 8       |
| Col 3      | Pin 7       |
| Col 4      | Pin 6       |

#### Other Components
| Component          | Arduino Pin |
|--------------------|-------------|
| Door Servo         | Pin 3       |
| Motion Servo       | Pin 5       |
| Temperature Sensor | A2          |
| Motion Sensor      | Pin 4       |
| LCD (SDA, SCL)     | A4, A5      |

---

### LPG & Flame Detection System

#### Components Connections
| Component        | Arduino Pin |
|------------------|-------------|
| LPG Sensor       | A1          |
| Flame Sensor     | A5          |
| Buzzer           | Pin 7       |
| Pump             | Pin 2       |

---

## Setup Instructions

1. Clone the repository:  
   ```bash
   git clone https://github.com/PronoyKumarMondal/Iot-Smart_home-Prroject
   ```
2. Open the respective project folder in the Arduino IDE:  
   - `door_control_system/door_control.ino`  
   - `lpg_flame_detection/lpg_flame.ino`  
3. Install the necessary libraries from the Arduino Library Manager:  
   - `Servo`  
   - `Keypad`  
   - `LiquidCrystal_I2C`  
   - `RemoteXY`  
4. Connect the components according to the circuit diagrams provided.  

---

## How to Upload Code

1. Connect your Arduino UNO to the computer using a USB cable.  
2. Open the appropriate `.ino` file in the Arduino IDE.  
3. Select the correct **Board** and **Port** under the **Tools** menu.  
4. Click the **Upload** button in the Arduino IDE to upload the code to the board.  
5. Test the system functionality.  

---
