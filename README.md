# Automatic_water_level_monitor

  # 🔧 Components Required:
  
  ESP32 Dev Board – Acts as the main controller to process water level data.

  HC-SR04 Ultrasonic Sensor – Measures the water level by detecting the distance to the water surface.

  I2C 16x2 LCD Display – Displays the water level percentage.

  I2C Module for LCD – Converts the LCD to an I2C interface (if not already integrated).

  Buzzer (Optional) – Sounds an alert when the water level is too low.

  Resistors (1KΩ and 2.2KΩ) – Used for voltage division to safely connect the HC-SR04's ECHO pin to ESP32.
  
  Jumper Wires – Required for making circuit connections.

  5V Power Source (USB or Adapter) – Supplies power to the ESP32 and other components.

  # 📌 Circuit Connections:
  
  # Connecting the HC-SR04 Ultrasonic Sensor to ESP32:
  
  Connect the VCC pin of the HC-SR04 to the 5V pin of the ESP32.  

  Connect the GND pin of the HC-SR04 to the GND pin of the ESP32.

  Connect the TRIG pin of the HC-SR04 to GPIO 5 of the ESP32.

  Connect the ECHO pin of the HC-SR04 to a voltage divider circuit (1KΩ + 2.2KΩ resistors) to reduce the voltage from 5V to 3.3V, then connect it to GPIO 18 of the ESP32.

  # Connecting the I2C LCD Display to ESP32:
  
  Connect the VCC pin of the I2C LCD to the 5V pin of the ESP32.

  Connect the GND pin of the I2C LCD to the GND pin of the ESP32.

  Connect the SDA pin of the I2C LCD to GPIO 21 of the ESP32.

  Connect the SCL pin of the I2C LCD to GPIO 22 of the ESP32.
  
  # Why ESP32 Instead of Arduino?
  
  ✔ Wi-Fi and Bluetooth support (Can be expanded for IoT monitoring).

  ✔ Faster processing than Arduino.

  ✔ More GPIOs & supports 3.3V sensors directly.

