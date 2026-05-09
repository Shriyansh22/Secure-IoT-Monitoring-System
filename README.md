# Secure-IoT-Monitoring-System

Real-time environmental monitoring using ESP8266, DHT11, and MQ-2 sensors with secure encrypted Wi-Fi communication, Flask backend processing, and a modern live dashboard for visualization and alerts.

---

# 📌 Overview

The **Secure IoT Monitoring System** is a lightweight and secure environmental monitoring platform designed for real-time sensing and alerting. The project combines embedded systems, wireless communication, cybersecurity concepts, and web technologies to create a reliable IoT solution.

The system continuously monitors:

- 🌡 Temperature
- 💧 Humidity
- 🔥 Gas / Smoke Levels

Sensor data is encrypted on the ESP8266 device using a lightweight XOR + Base64 encryption mechanism before being transmitted over Wi-Fi to a Flask backend server. The server decrypts, validates, logs, and visualizes the data through a responsive dashboard.

---

# 🚀 Features

- ✅ Real-time environmental monitoring
- ✅ Secure XOR + Base64 encrypted transmission
- ✅ ESP8266 Wi-Fi communication
- ✅ Flask-based backend server
- ✅ Live Chart.js dashboard
- ✅ Gas leakage & smoke detection
- ✅ LED + buzzer alert system
- ✅ Auto-refresh dashboard
- ✅ CSV data logging
- ✅ Downloadable monitoring reports
- ✅ Dark / Light dashboard theme
- ✅ Responsive web interface

---

# 🛠 Hardware Components

| Component | Description |
|---|---|
| ESP8266 NodeMCU | Main IoT microcontroller |
| DHT11 | Temperature & humidity sensor |
| MQ-2 | Gas & smoke sensor |
| LED | Visual alert |
| Buzzer | Audio alert |
| 16×2 I2C LCD | Local display module |
| Breadboard & Jumper Wires | Hardware connections |

---

# 💻 Software Stack

| Technology | Usage |
|---|---|
| Arduino IDE | ESP8266 firmware |
| Python | Backend development |
| Flask | Web server |
| HTML/CSS/JS | Dashboard UI |
| Chart.js | Real-time graphs |
| JSON | Data exchange |
| XOR + Base64 | Lightweight encryption |

---

# 📡 System Architecture

```text
DHT11 + MQ-2 Sensors
          ↓
     ESP8266 NodeMCU
          ↓
 XOR + Base64 Encryption
          ↓
      Wi-Fi Network
          ↓
      Flask Backend
          ↓
 Real-Time Dashboard
          ↓
  LED + Buzzer Alerts
```

---

# 🔐 Security Mechanism

The project implements a lightweight security layer using:

- XOR encryption
- Base64 encoding
- Local Wi-Fi communication
- Backend-side decryption and validation

This approach prevents plain-text transmission of sensor readings and demonstrates secure communication principles in embedded IoT systems.

---

# 📊 Dashboard Features

The web dashboard includes:

- Live sensor values
- Temperature charts
- Humidity trends
- Gas level monitoring
- Threshold-based alerts
- Device online/offline status
- Auto-refresh updates
- Downloadable PDF reports

---

# ⚡ Hardware Connections

| Sensor / Module | NodeMCU Pin |
|---|---|
| DHT11 DATA | D4 |
| MQ-2 Analog Output | A0 |
| LCD SDA | D2 |
| LCD SCL | D1 |
| LED | D6 |
| Buzzer | D7 |

---

# 📂 Project Structure

```bash
Secure-IoT-Monitoring-System/
│
├── esp8266_code/
│   └── secure_iot.ino
│
├── flask_server/
│   ├── app.py
│   ├── templates/
│   ├── static/
│   └── logs/
│
├── dashboard/
│   └── dashboard.html
│
├── images/
│   ├── architecture.png
│   ├── dashboard.png
│   └── wiring.png
│
├── report/
│   └── Project_Report.pdf
│
└── README.md
```

---

# ▶️ Installation & Setup

## 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/Secure-IoT-Monitoring-System.git
cd Secure-IoT-Monitoring-System
```

---

## 2️⃣ Install Python Dependencies

```bash
pip install flask pandas matplotlib
```

---

## 3️⃣ Upload ESP8266 Firmware

- Open Arduino IDE
- Install ESP8266 board package
- Install required libraries:
  - DHT Sensor Library
  - LiquidCrystal_I2C
  - ESP8266WiFi
- Upload firmware to NodeMCU

---

## 4️⃣ Start Flask Server

```bash
python app.py
```

---

## 5️⃣ Open Dashboard

```text
http://127.0.0.1:5000
```

---

# 📈 Sample Output

- Real-time sensor readings
- Gas leak alerts
- Interactive charts
- LCD display updates
- Audio + visual warning system

---

# 🎯 Applications

- Smart homes
- Industrial safety systems
- Gas leakage monitoring
- Environmental monitoring
- IoT security research
- Educational embedded projects

---

# 🔮 Future Improvements

- MQTT protocol integration
- AES/TLS encryption
- Cloud synchronization
- Mobile application
- Multi-device monitoring
- AI-based anomaly detection
- Push notifications

---

# 👨‍💻 Contributors

- Shriyansh Chaudhary
- Harshit Gupta
- Anjali Raj
- Shivanand
- Anupam Chaurasiya

---

# 📚 References

- ESP8266 Documentation
- DHT11 Datasheet
- MQ-2 Sensor Datasheet
- Flask Documentation
- Chart.js Documentation

---

# 📜 License

This project is developed for academic and educational purposes under the Faculty of Technology, University of Delhi.

---

# ⭐ Support

If you found this project useful:

- ⭐ Star the repository
- 🍴 Fork the project
- 🛠 Contribute improvements

---

# 📧 Contact

**Shriyansh Chaudhary**  
