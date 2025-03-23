# Air Quality Monitoring System using NodeMCU, DHT11, MQ135 Sensor, and Arduino IoT Cloud

## Introduction
This project is an IoT-based Air Quality Monitoring System that uses a NodeMCU ESP8266, DHT11 sensor, and MQ135 gas sensor to measure air quality parameters such as temperature, humidity, and air pollution levels. The data is transmitted to the Arduino IoT Cloud platform, where it can be monitored in real time through a dashboard.

## Features
- **Real-time Monitoring:** Continuously measures air quality, temperature, and humidity.
- **Cloud Integration:** Sends data to the Arduino IoT Cloud for remote monitoring.
- **Dashboard Visualization:** Displays sensor data using widgets such as gauges, graphs, and messenger notifications.
- **WiFi Connectivity:** Uses NodeMCU ESP8266 to connect to the internet and send data.
- **User Alerts:** Can trigger alerts when air quality exceeds safe levels.

## Components Used
1. **NodeMCU ESP8266** - Microcontroller with WiFi capability.
2. **DHT11 Sensor** - Measures temperature and humidity.
3. **MQ135 Gas Sensor** - Detects air pollutants such as CO2, ammonia, benzene, and smoke.
4. **I2C LCD Display (Optional)** - Displays real-time data locally.
5. **Jumper Wires** - For connections.
6. **Power Supply** - 5V USB or battery.

## Circuit Connections
- **MQ135 Sensor:**
  - A0 -> NodeMCU A0
  - GND -> NodeMCU GND
  - VCC -> NodeMCU 3V

- **DHT11 Sensor:**
  - OUT -> NodeMCU D2 (GPIO 4)
  - GND -> NodeMCU GND
  - VCC -> NodeMCU 3V

- **I2C LCD Display (Optional):**
  - SDA -> NodeMCU D3 (GPIO 0)
  - SCL -> NodeMCU D1 (GPIO 5)
  - VCC -> NodeMCU 3V
  - GND -> NodeMCU GND

## Software Requirements
- **Arduino IDE** - For writing and uploading code.
- **Arduino IoT Cloud** - For cloud-based monitoring.
- **ESP8266WiFi Library** - Enables WiFi connectivity.
- **DHT Library** - Reads data from the DHT11 sensor.
- **MQ135 Library** - Reads air quality data.
- **LiquidCrystal_I2C Library (Optional)** - For LCD display.

## Setup & Configuration
1. **Install Required Libraries:**
   - Open Arduino IDE and install `ESP8266WiFi`, `DHT sensor library`, `MQ135`, and `LiquidCrystal_I2C`.
2. **Create an Arduino IoT Cloud Account:**
   - Add a new device (NodeMCU ESP8266) and create variables for `temperature`, `humidity`, and `air_quality`.
3. **Configure WiFi Credentials:**
   - Set your WiFi SSID and password in the code.
4. **Upload Code to NodeMCU:**
   - Connect NodeMCU via USB and upload the `.ino` file.
5. **Monitor Data:**
   - Open Arduino IoT Cloud Dashboard to view real-time sensor data.

## Usage
- Power the NodeMCU and allow it to connect to WiFi.
- Open the Arduino IoT Cloud dashboard to monitor air quality data.
- If using an LCD display, it will show real-time sensor readings locally.
- Set alerts if air quality levels exceed safe thresholds.

## Future Enhancements
- Implement mobile notifications for alerts.
- Store historical data for trend analysis.
- Add more sensors for better accuracy.
- Develop a mobile app for real-time monitoring.

## Contribution
Feel free to contribute by improving the code, adding features, or suggesting enhancements!

## License
This project is open-source and free to use for educational and personal purposes.

---

**Author:** Swastik Mishra  
**Email:** theswastikmishraofficial@gmail.com  
**LinkedIn:** [Swastik Mishra](https://www.linkedin.com/in/myselfswastikmishra)
