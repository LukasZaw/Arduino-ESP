# ESP8266 Projects

Welcome to the ESP8266 Projects repository! This repository contains various projects utilizing the ESP8266 microcontroller for IoT applications, home automation, and more.


## 🚀 Projects
Below is a list of projects included in this repository:

### 1. [Dallas Web Server](projects/dallas_webserver)
- **Description:** This project is a web-based temperature monitoring system using an ESP8266 and a DS18B20 temperature sensor. The temperature data is updated dynamically using AJAX requests.
- **Features:**
  - Reads temperature data from a DS18B20 sensor.
  - Hosts a web server on ESP8266/ESP32 to display real-time temperature readings.
  - Uses AJAX to update temperature values without refreshing the page.
  - Displays data in both Celsius and Fahrenheit.
  - Connects to Wi-Fi for remote monitoring.



## 🔒 Managing Wi-Fi Credentials
To keep your Wi-Fi credentials secure, I used a separate configuration file:
1. Create a file named `config.h` in your project folder.
2. Add the following content:
   ```cpp
   #ifndef CONFIG_H
   #define CONFIG_H

   const char* ssid = "your-SSID";
   const char* password = "your-PASSWORD";

   #endif
   ```
3. Include this file in your main source file:
   ```cpp
   #include "config.h"
   ```
4. Add `config.h` to `.gitignore` to prevent it from being uploaded to GitHub:
   ```
   config.h
   ```

## 📚 Used for Projects
- ESP8266-based board (ESP-12E NodeMCU)
- Arduino IDE and VS Code
- Required libraries
- Sensors and modules as specified per project
