# 🌦️ Smart Weather Monitor

This project is an IoT-based environmental monitoring system that reads air quality and carbon monoxide levels using gas sensors (MQ135 and MQ7), displays the data on an LCD screen, and uploads it to the cloud using the ESP8266 Wi-Fi module. It is ideal for smart city and indoor air quality monitoring applications.

---

## 🔧 Features

- Measures:
  - 🌫️ Air Quality (MQ135)
  - ☠️ Carbon Monoxide Levels (MQ7)
  - 🌡️ Temperature & Humidity (optional)
- Displays readings on an LCD (16x2) screen
- Sends real-time data to the ThingSpeak IoT cloud
- Expandable with additional sensors like DHT11, BMP180, etc.

---

## 🛠️ Hardware Components

| Component          | Quantity | Description                            |
|--------------------|----------|----------------------------------------|
| Arduino UNO        | 1        | Main microcontroller                   |
| ESP8266 Wi-Fi      | 1        | Sends data to the internet             |
| MQ135              | 1        | Gas sensor for air quality             |
| MQ-7               | 1        | Gas sensor for carbon monoxide         |
| LCD 16x2 (I2C)     | 1        | Displays sensor readings               |
| Breadboard         | 1        | For circuit building                   |
| Jumper Wires       | Many     | For making connections                 |
| Power Supply       | 1        | USB power or battery source            |

---

## 📐 Circuit Diagram

Here’s the full circuit wiring used in this project:

![Circuit Diagram](circuit_diagram.png)

---

## 📲 Cloud Dashboard

You can connect this system to [ThingSpeak](https://thingspeak.com) and view your real-time sensor data.

---

## 🚀 How to Use

1. **Clone the Repo**
   ```bash
   git clone https://github.com/kavya0457/smart-weather-monitor.git
   cd smart-weather-monitor
Open Arduino IDE

Open code/main.ino (or your .ino file)

Select Board: Arduino UNO

Select Port

Install Required Libraries

ESP8266WiFi

ThingSpeak

LiquidCrystal_I2C (for the LCD)

Adafruit Sensor (optional if using DHT/BMP sensors)

Edit the Wi-Fi Credentials & API Key in the Code

const char* ssid = "your_wifi_name";
const char* password = "your_wifi_password";
const char* writeAPIKey = "your_thingspeak_api_key";

Upload the Code

Connect Arduino UNO via USB
Upload and monitor via Serial Monitor

📸 Screenshots
<img width="909" height="532" alt="circuit diagram png" src="https://github.com/user-attachments/assets/a459e07d-662e-43fa-85f7-ff64409b9aca" />


📝 License
This project is licensed under the MIT License.

🙋‍♀️ Author
Kavya0457

If you like this project, give it a ⭐ on GitHub!

