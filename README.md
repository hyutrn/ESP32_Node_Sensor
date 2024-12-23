| Supported Targets | ESP32 | ESP32-C2 | ESP32-C3 | ESP32-C6 | ESP32-H2 | ESP32-S2 | ESP32-S3 |
| ----------------- | ----- | -------- | -------- | -------- | -------- | -------- | -------- |

# ESP32 IoT Sensor with OLED Display and MQTT

This project demonstrates an IoT sensor system built on ESP32 that reads data from sensors (like temperature, humidity, and light sensors), displays the information on an OLED screen, and communicates with a server using MQTT.

## Features

- **OLED Display**: Displays sensor data on a 128x64 SSD1306 OLED display with scrolling text.
- **Button Controls**: Two buttons for restarting and resetting the system.
- **Wi-Fi**: Connects to a Wi-Fi network to send data to a server.
- **HTTP Server**: Create a webserver to config node ESP32
- **MQTT**: Publishes sensor data to a remote MQTT broker.
- **Sensor Support**: Reads from DHT11 (Temperature and Humidity), Light Sensor, and Moisture Sensor.

## Hardware Requirements

- **ESP32 Development Board**
- **OLED Display**: SSD1306, connected via I2C
- **DHT11 Sensor**: For temperature and humidity readings
- **Light Sensor** 
- **Moisture Sensor** 
- **2 Push Buttons**: For reset and restart functionality

## Pin Configuration

- **I2C Pins**:
  - SDA: GPIO 21
  - SCL: GPIO 22
- **Buttons**:
  - BUTTON_1: GPIO 27 (Reset)
  - BUTTON_2: GPIO 26 (Restart)

## Software Requirements

- **ESP-IDF**: ESP32 development framework.
- **LVGL**: Lightweight Graphics Library for UI.
- **MQTT Library**: For MQTT communication.

## Setup and Installation

### 1. Install ESP-IDF

Follow the instructions from the official [ESP-IDF setup guide](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/) to install the ESP-IDF development environment.

### 2. Clone the Repository

Clone this repository to your local machine:

```bash
git clone <repository-url>
cd <repository-folder>

