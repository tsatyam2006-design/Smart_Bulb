# ESP32 Smart Bulb Control with PIR Sensor

A simple home automation project using **ESP32, a 2-channel relay module, and a PIR motion sensor** to control two bulbs through a web interface.

## ✨ Features

* 📱 Web-based bulb control using a smartphone or computer.
* 💡 Bulb 1: Manual control + automatic PIR motion detection.
* 💡 Bulb 2: Manual control only.
* 📶 Wi-Fi Access Point mode — no external router or internet required.

## 🛠️ Components Required

* ESP32 Development Board
* 2-Channel Relay Module
* PIR Motion Sensor (HC-SR501 or equivalent)
* 2 Bulbs with suitable power supplies
* Jumper Wires

## 🔌 Pin Connections

| Component        | ESP32 GPIO |
| ---------------- | ---------- |
| Relay 1 (Bulb 1) | GPIO 26    |
| Relay 2 (Bulb 2) | GPIO 27    |
| PIR Sensor OUT   | GPIO 25    |

## 🚀 How to Use

1. Upload the code to your ESP32 using Arduino IDE.
2. Connect to the Wi-Fi network:

   * **SSID:** `ESP32_Control`
   * **Password:** `12345678`
3. Open a browser and visit `192.168.4.1`.
4. Use the buttons to control both bulbs.

## 💻 Technologies Used

* Arduino IDE
* ESP32 Wi-Fi
* WebServer Library
* PIR Motion Detection

## ⚠️ Note

The relay module in this code is **active-LOW**. Bulb 1 can be switched on by motion detection even when its manual state is OFF.

**Safety:** Take proper precautions when working with AC mains voltage.

## 📜 License

This project is open-source and available for learning and personal use.
