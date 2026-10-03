# IoT-Based Real-Time Monitoring of Food Additives and Preservatives

An IoT-based food quality monitoring project using **NodeMCU ESP8266, pH Sensor, TDS Sensor, DHT22, and ThingSpeak** to collect and visualize sensor data in real time.

## 📌 About the Project

This project was developed as an academic IoT project to explore how sensors and cloud-based platforms can be used for monitoring food-related parameters.

The system uses multiple sensors connected to a **NodeMCU ESP8266**. The collected readings are sent through Wi-Fi to **ThingSpeak**, where they can be stored and visualized using real-time graphs.

The current ThingSpeak channel records:

- 🌡️ Temperature
- 💧 Humidity
- 🧪 pH
- 📊 TDS Sensor Level

## 🎯 Objectives

- Develop an IoT-based food monitoring prototype.
- Collect food-related sensor readings in real time.
- Monitor pH and TDS levels of samples.
- Record temperature and humidity along with the sensor readings.
- Send sensor data to a cloud platform using Wi-Fi.
- Visualize the collected data remotely using ThingSpeak.

## 🔧 Hardware Components

- **NodeMCU ESP8266**
- **pH Sensor**
- **TDS Sensor**
- **DHT22 Temperature & Humidity Sensor**
- **Jumper Wires**
- **Breadboard**
- **Buzzer** *(if used in the final prototype)*

## 💻 Software & Technologies

- Arduino IDE
- C/C++
- ESP8266
- Internet of Things (IoT)
- Wi-Fi
- ThingSpeak

## ⚙️ Working Principle

The system follows the flow:

```text
             Food Sample
                  │
                  ▼
        ┌──────────────────┐
        │     Sensors      │
        │                  │
        │  pH Sensor       │
        │  TDS Sensor      │
        │  DHT22           │
        └────────┬─────────┘
                 │
                 ▼
        ┌──────────────────┐
        │ NodeMCU ESP8266  │
        │                  │
        │ Data Processing  │
        │ Wi-Fi Connection │
        └────────┬─────────┘
                 │
                 │ Internet
                 ▼
        ┌──────────────────┐
        │    ThingSpeak    │
        │      Cloud       │
        └────────┬─────────┘
                 │
                 ▼
        ┌──────────────────┐
        │  Online Graphs   │
        │  & Data Monitor  │
        └──────────────────┘
