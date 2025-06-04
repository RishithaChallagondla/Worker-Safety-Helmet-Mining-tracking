# Worker Safety Helmet & Mining Tracking System

An Iot-based Smart helmet for real-time worker safety and location tracking in mining environments. This project uses an ESP32, various sensors, and Blynk to monitor dangerous conditions like gas leaks, temperature, and metal hazards — and sends alerts instantly.

##  Components Used

- ESP32 Development Board
- MQ-135 Gas Sensor – detects harmful gases
- DHT11 Temperature Sensor – monitors heat levels
- GY-NEO6MV2 GPS Module– tracks worker location
- 16x2 LCD Display (with I2C) – shows data
- Metal Detector Sensor – detects buried metals
- Buzzer – gives safety alerts
- Blynk App – receives alerts on smartphone

##  Features

-  Sends alerts on detecting toxic gas(concentration range exceeds) or high temperature
-  Tracks worker’s GPS location in real-time
-  Detects presence of underground metals
-  Smartphone alert via Blynk IoT
-  Displays live values on LCD

##  How It Works

1. Sensors continuously monitor the environment.
2. If any value crosses the threshold (e.g., gas, heat):
   - A buzzer rings
   - Data is shown on the LCD
   - Worker’s phone receives an alert via Blynk
3. Location is tracked using GPS and displayed on Blynk

##  Circuit Connections

> Detailed circuit diagram is available in the /images/ folder.

- MQ-135: DO → D34, VCC → 3V3, GND → GND  
- DHT11: DAT → D4, VCC → 3V3, GND → GND  
- LCD (I2C): SDA → D21, SCL → D22  
- GPS: TX → GPIO17, RX → GPIO16  
- Buzzer: VCC → 3V3, GND → GND  
