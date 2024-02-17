# DHT11 Temperature and Humidity Sensor Display

This Arduino code reads temperature and humidity data from a DHT11 sensor and displays it on an OLED screen.

## Description
The code initializes a DHT11 sensor and an OLED display. It continuously reads temperature and humidity data from the sensor and displays it both on the Serial Monitor and the OLED display.

## Dependencies
- [DHT Sensor Library](https://github.com/adafruit/DHT-sensor-library)
- [Adafruit GFX Library](https://github.com/adafruit/Adafruit-GFX-Library)
- [Adafruit SSD1306 Library](https://github.com/adafruit/Adafruit_SSD1306)

## Hardware Requirements
- Arduino board
- DHT11 sensor
- OLED display (128x64 pixels)

## Pin Configuration
- DHT11 sensor:
  - Signal pin: Pin 2
- OLED display:
  - DC pin: Pin 9
  - CS pin: Pin 10
  - RESET pin: Pin 11

## Instructions
1. Connect the DHT11 sensor and OLED display to the Arduino board according to the specified pin configuration.
2. Upload this code to your Arduino board.
3. Open the Serial Monitor to view temperature and humidity readings.
4. The OLED display will also show the temperature and humidity data.

## Functions
- `setup()`: Initializes serial communication, DHT sensor, and OLED display.
- `loop()`: Reads temperature and humidity data from the DHT sensor and displays it on both Serial Monitor and OLED display.
- `oledDisplayHeader()`: Displays the header on the OLED display.
- `oledDisplay()`: Displays temperature and humidity values on the OLED display.

## License
This code is released under the [MIT License](LICENSE).
