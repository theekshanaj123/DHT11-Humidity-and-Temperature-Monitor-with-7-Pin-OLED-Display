# DHT11 Humidity and Temperature Monitor with OLED Display

This Arduino project allows you to monitor humidity and temperature using the DHT11 sensor and display the values on an OLED display. The project utilizes the Adafruit SSD1306 library for controlling the OLED display and the DHT sensor library for interfacing with the DHT11 sensor.

## Requirements

- Arduino board (e.g., Arduino Uno)
- DHT11 humidity and temperature sensor
- SSD1306 OLED display
- Jumper wires

## Dependencies

- [Adafruit GFX Library](https://github.com/adafruit/Adafruit-GFX-Library)
- [Adafruit SSD1306 Library](https://github.com/adafruit/Adafruit_SSD1306)
- [DHT Sensor Library](https://github.com/adafruit/DHT-sensor-library)

Make sure to install these libraries in your Arduino IDE before uploading the code.

## Hardware Setup

1. **Connect the DHT11 sensor to your Arduino board:**
   - Connect the positive (red) pin of the DHT11 to the 5V pin on the Arduino.
   - Connect the negative (black) pin of the DHT11 to the GND pin on the Arduino.
   - Connect the signal (data) pin of the DHT11 to digital pin 2 on the Arduino.

2. **Connect the SSD1306 OLED display:**
   - Connect the MOSI pin of the OLED display to digital pin 9 on the Arduino.
   - Connect the CLK pin of the OLED display to digital pin 10 on the Arduino.
   - Connect the DC pin of the OLED display to digital pin 11 on the Arduino.
   - Connect the CS pin of the OLED display to digital pin 12 on the Arduino.
   - Connect the RESET pin of the OLED display to digital pin 13 on the Arduino.
   - Connect the VCC pin of the OLED display to the 5V pin on the Arduino.
   - Connect the GND pin of the OLED display to the GND pin on the Arduino.
  
## Hardware Setup

| **Component**                   | **Arduino Pin** |
|--------------------------------|-----------------|
| DHT11 Sensor                    |                 |
| Positive (Red) Pin              | 5V              |
| Negative (Black) Pin            | GND             |
| Signal (Data) Pin               | Digital Pin 2   |
|                                |                 |
| SSD1306 OLED Display            |                 |
| MOSI Pin                        | Digital Pin 9   |
| CLK Pin                         | Digital Pin 10  |
| DC Pin                          | Digital Pin 11  |
| CS Pin                          | Digital Pin 12  |
| RESET Pin                       | Digital Pin 13  |
| VCC Pin                         | 5V              |
| GND Pin                         | GND             |


## Usage

1. **Upload the provided code to your Arduino board.**
   - Open the Arduino IDE.
   - Connect your Arduino board to your computer using a USB cable.
   - Open the Arduino sketch file (.ino) in the IDE.
   - Click the "Upload" button to compile and upload the code to your Arduino board.

2. **Open the serial monitor to view the humidity and temperature readings.**
   - After uploading the code, open the serial monitor in the Arduino IDE.
   - Set the baud rate to 9600.
   - You will see the humidity and temperature readings printed in the serial monitor.

3. **View real-time readings on the OLED display.**
   - The OLED display will show the current humidity and temperature readings in real-time.
   - If the readings are not displayed correctly, check the connections and make sure the libraries are installed correctly.

## Notes

- **Adjust DHT Settings:** Make sure to adjust the `DHTPIN` and `DHTTYPE` constants in the code according to your setup if you're using a different pin or a different DHT sensor model.
- **Display Configuration:** You may need to adjust the `SCREEN_WIDTH`, `SCREEN_HEIGHT`, and pin definitions for the OLED display if you're using a different display model or wiring configuration.
- **Display Connection:** This code is set to use the default software SPI connection for the OLED display. If you're using hardware SPI or I2C, you'll need to modify the display initialization accordingly.
- **Troubleshooting:** If you encounter any issues, double-check the hardware connections, ensure libraries are correctly installed, and consult the serial monitor for debugging information.

