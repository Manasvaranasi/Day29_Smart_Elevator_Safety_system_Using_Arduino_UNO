# 🛗 Smart Elevator Safety System

## 📌 Project Description

The Smart Elevator Safety System is an Arduino UNO based embedded project designed to improve elevator safety by monitoring door clearance and passenger load in real time.

The system uses an HC-SR04 Ultrasonic Sensor to detect obstacles near the elevator door and a Force Sensor (FSR) to monitor elevator load. Based on sensor readings, the system classifies the elevator status into Safe, Warning, or Critical conditions and provides alerts using LEDs, a buzzer, and an LCD display.

This project demonstrates how embedded systems can enhance elevator safety in residential, commercial, and industrial buildings.

---

## 🚀 Features

- Real-Time Elevator Safety Monitoring
- Door Obstacle Detection
- Passenger Load Monitoring
- LCD Status Display
- Visual Alert System
- Audible Warning Alarm
- Safe, Warning & Critical Status Indication
- Smart Building Safety Concept

---

## 🛠 Components Used

- Arduino UNO
- HC-SR04 Ultrasonic Sensor
- Force Sensor (FSR)
- LCD 16×2 Display
- Green LED
- Yellow LED
- Red LED
- Piezo Buzzer
- 10kΩ Resistor
- 220Ω Resistors
- Breadboard
- Jumper Wires

---

## 🔌 Circuit Connections

### HC-SR04 Ultrasonic Sensor

| Pin | Arduino |
|------|----------|
| VCC | 5V |
| GND | GND |
| TRIG | D8 |
| ECHO | D9 |

---

### Force Sensor (FSR)

| Force Sensor | Arduino |
|--------------|----------|
| Terminal 1 | 5V |
| Terminal 2 | A0 |
| Terminal 2 | 10kΩ → GND |

---

### LEDs

#### Green LED

| LED | Arduino |
|------|----------|
| Anode (+) | D3 |
| Cathode (-) | 220Ω → GND |

#### Yellow LED

| LED | Arduino |
|------|----------|
| Anode (+) | D4 |
| Cathode (-) | 220Ω → GND |

#### Red LED

| LED | Arduino |
|------|----------|
| Anode (+) | D5 |
| Cathode (-) | 220Ω → GND |

---

### Piezo Buzzer

| Buzzer | Arduino |
|---------|----------|
| Positive (+) | D6 |
| Negative (-) | GND |

---

### LCD 16×2 Display

| LCD Pin | Arduino |
|----------|----------|
| VSS | GND |
| VDD | 5V |
| VO | GND |
| RS | D12 |
| RW | GND |
| E | D11 |
| D4 | A1 |
| D5 | A2 |
| D6 | A3 |
| D7 | A4 |
| A | 5V |
| K | GND |

---

## ⚙️ Working Principle

The system continuously monitors the elevator door area and passenger load.

### 🟢 Safe Condition

Conditions

- Distance > 100 cm
- Force Sensor < 400

Actions

- Green LED ON
- Buzzer OFF
- LCD Displays Safe Status

LCD Output

```text
STATUS: SAFE
DOOR CLEAR
```

---

### 🟡 Warning Condition

Conditions

- Distance between 50 cm and 100 cm
- OR Force Sensor between 400 and 700

Actions

- Yellow LED ON
- Buzzer OFF
- LCD Displays Warning Status

LCD Output

```text
WARNING
CHECK DOOR
```

---

### 🔴 Critical Condition

Conditions

- Distance < 50 cm
- OR Force Sensor > 700

Actions

- Red LED ON
- Buzzer ON
- LCD Displays Critical Alert

LCD Output

```text
CRITICAL!
STOP ELEVATOR
```

---

## 🏢 Applications

- Residential Elevators
- Commercial Buildings
- Hospitals
- Shopping Malls
- Hotels
- Industrial Lifts
- Smart Building Automation

---

## 📚 Learning Outcomes

- Arduino Programming
- Ultrasonic Sensor Interfacing
- Force Sensor Interfacing
- LCD Programming
- Safety System Design
- Embedded Systems Development
- Building Automation Concepts

---

## 🔮 Future Enhancements

- ESP32 IoT Monitoring
- Mobile App Notifications
- RFID User Authentication
- Emergency SMS Alerts
- Elevator Floor Monitoring
- Cloud-Based Data Logging
- Voice Announcements
- AI-Based Predictive Maintenance

---

## 👨‍💻 Author

**MANAS VARANASI**

### 🚀 Day 29 of 45 Days Embedded Systems & Electronics Challenge

### 🛗 Project: Smart Elevator Safety System

Building One Project Every Day To Strengthen My Embedded Systems, IoT, and Automation Skills.

---

## 📂 Repository Information

**Repository Name**

day29-smart-elevator-safety-system

**Code File**

Smart_Elevator_Safety_System.ino

**Circuit Name**

Smart Elevator Safety System Circuit

**Project Type**

Embedded Systems | Smart Building | Arduino Project