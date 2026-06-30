# FPGA-based-Home-Automation-System


An innovative **real-time Smart Home Automation System** designed and implemented on a **Field-Programmable Gate Array (FPGA)** using **Verilog HDL**. This project was developed as the final project for the **Digital Electronics Laboratory (EEE 304)** at the **Bangladesh University of Engineering and Technology (BUET)**.

Unlike conventional microcontroller-based solutions, this design leverages the inherent parallelism of FPGA technology to provide **low-latency operation**, **hardware scalability**, and **enhanced reliability** for home automation applications.

---

## 🚀 Features

### 🔒 Secure Password Authentication
- 4-bit password-based access control.
- Correct password opens the main gate.
- Automatically activates the corridor light upon successful authentication.

### ⏳ Automated Corridor Lighting
- Corridor light remains ON for **10 seconds** after entry.
- Turns OFF automatically without user intervention.

### 👥 Real-Time Occupancy Detection
- Uses dual IR sensors to accurately detect entry and exit.
- Implements Finite State Machine (FSM)-based occupancy counting.
- Prevents false counting due to improper sensor triggering.

### 💡 Intelligent Room Lighting
- Room light automatically turns ON when occupancy is detected.
- Turns OFF immediately when the room becomes empty.

### 🌡️ Adaptive Fan Control
- Monitors ambient temperature using an NTC thermistor.
- Fan activates when the temperature exceeds **30°C**.
- PWM-based speed control according to occupancy:
  - **25% Duty Cycle**
  - **50% Duty Cycle**
  - **75% Duty Cycle**
  - **100% Duty Cycle**

### ♻️ Energy-Efficient Shutdown
- Automatically switches OFF all appliances when the last occupant leaves.
- Resets the occupancy counter to eliminate unnecessary power consumption.

---

# 🛠 System Architecture

The system is controlled using two dedicated **Finite State Machines (FSMs)** for reliable entry and exit detection.

## Entry Sequence

<img width="928" height="476" alt="image" src="https://github.com/user-attachments/assets/84ae28cf-b656-4648-acf2-07d6b232a1a9" />


## Exit Sequence

<img width="928" height="324" alt="image" src="https://github.com/user-attachments/assets/555e6832-0e8d-4608-81c9-23633a4edcb5" />


---

# 🔄 Overall System Flow

<img width="928" height="1000" alt="image" src="https://github.com/user-attachments/assets/03f327cc-4f1b-41ca-a3c9-2ad1bf333006" />

---



---

# ⚙️ Getting Started

## Clone the Repository

```bash
git clone https://github.com/ifat-azwad/FPGA-based-Home-Automation-System.git
```

## Open the Project

Open the project using **Intel Quartus Prime** (or any compatible FPGA development environment).

## Compile & Synthesize

- Import the Verilog source files 
- Compile and synthesize the project.

## Configure FPGA Pins

Assign the FPGA I/O pins for:

- IR Sensors
- NTC Temperature Sensor
- PWM Output
- 7-Segment Display
- LEDs
- Push Buttons

according to your FPGA development board.

## Program the FPGA

Generate the `.sof` or `.pof` programming file and flash it onto the FPGA board.

---

# 🔮 Future Work

- 🎤 Voice-controlled home automation
- 📱 ESP32/Wi-Fi based mobile application
- ☁️ IoT cloud monitoring
- 🚨 Intrusion detection and security alarms
- 📊 Energy consumption monitoring
- 🌞 Smart energy optimization

---


# 🎥 Project Demonstration

📺 **Video Demo:** https://youtu.be/kKojmWgY1q4

---


