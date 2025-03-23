# Automatic_water_level_monitor
Here is the ESP32-based Automatic Water Level Monitor using an Ultrasonic Sensor (HC-SR04). This version will display the water level on the Serial Monitor and an OLED Display (SSD1306, optional).

Components Required:
ESP32

HC-SR04 Ultrasonic Sensor

SSD1306 0.96" OLED Display (Optional)

Buzzer (Optional for alert)

Jumper Wires

Circuit Connections:
HC-SR04 Ultrasonic Sensor

VCC → 3.3V (ESP32)

GND → GND

Trig → GPIO 5

Echo → GPIO 18 (Use a voltage divider to step down 5V to 3.3V)

SSD1306 OLED Display (I2C)

VCC → 3.3V

GND → GND

SDA → GPIO 21

SCL → GPIO 22

Buzzer (Optional)

+ve → GPIO 15

GND → GND

How It Works:
ESP32 reads distance from the HC-SR04 Ultrasonic Sensor.

Calculates water level as a percentage of tank capacity.

Displays the water level on Serial Monitor & OLED Display.

If the water level is below 20%, the buzzer alerts.

Why ESP32 Instead of Arduino?
✔ Wi-Fi and Bluetooth support (Can be expanded for IoT monitoring).
✔ Faster processing than Arduino.
✔ More GPIOs & supports 3.3V sensors directly.

Let me know if you need modifications, like Wi-Fi monitoring via a web dashboard! 🚀💧
