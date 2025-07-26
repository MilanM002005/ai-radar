 AI Radar System with Arduino UNO 

This project simulates a real-time radar system using an **ultrasonic sensor**, **servo motor**, and **Arduino UNO**, displaying the distance of surrounding objects within a 180° sweep. The radar visualization is displayed on your PC using **Processing**.

---

📦 Features

- 180° servo-controlled radar sweep
- Real-time object detection using ultrasonic sensor (HC-SR04)
- Graphical radar interface via **Processing**
- Serial communication between Arduino and PC
- Visualized distance + angle on screen
- Customizable range and sweep angles

---

## 🔧 Components Used

| Component            | Description                        |
|---------------------|------------------------------------|
| 🧠 Arduino UNO       | Microcontroller board              |
| 📡 HC-SR04           | Ultrasonic distance sensor         |
| 🔄 SG90 Servo Motor  | For rotating the ultrasonic sensor |
| 🧵 Jumper Wires      | To connect everything              |
| 🔋 (Optional) 5V Power | For powering servo externally     |
| 💻 PC with Processing | To visualize the radar display     |
| 🔌 USB Cable         | For programming and serial comm.   |

---

## ⚙️ Wiring Instructions

### Ultrasonic Sensor (HC-SR04)

| HC-SR04 Pin | Arduino UNO Pin |
|-------------|------------------|
| VCC         | 5V               |
| GND         | GND              |
| Trig        | D8               |
| Echo        | D9               |

### Servo Motor (SG90)

| Servo Wire  | Arduino UNO Pin |
|-------------|------------------|
| Signal      | D10              |
| VCC         | 5V (or ext 5V)   |
| GND         | GND              |


  Software Used

- **Arduino IDE** (for uploading sketch)
- **Processing IDE** (for radar visualization)


 Getting Started

### 1. Upload Arduino Code
Upload the provided `arduino_radar.ino` sketch to your Arduino UNO using the Arduino IDE.

### 2. Run Processing Code
Open `radar_display.pde` in **Processing** IDE.  
Make sure to match the serial port in this line:
```java
myPort = new Serial(this, "COM5", 9600);
