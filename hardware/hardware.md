Parts:

### Arduino Nano
 - What microcontroller does it use?
    - The Arduino Nano uses the ATmega328P, an 8-bit microcontroller made by Microchip (formerly Atmel). It runs the Arduino program and controls all connected components

 - Operating voltage: 5 V

 - Digital pins: 14 digital input/output pins (D0–D13)

 - Analog pins: 8 analog input pins (A0–A7)

### MAX30102 Heart Rate Sensor
 - What does it actually measure?
    - The MAX30102 measures changes in blood flow using light. It estimates heart rate by detecting blood volume changes in your fingertip. It can also estimate blood oxygen saturation (SpO₂), although this project will focus on heart rate

 - How does it communicate?
    - It communicates with the Arduino using the I²C protocol, which only requires two data lines: SDA and SCL

 - Why are there two LEDs inside?
    - The sensor contains a red LED and an infrared (IR) LED. The IR LED is mainly used for heart-rate detection, while the red LED is used together with the IR LED to estimate blood oxygen levels (SpO₂)

 - Which Arduino library is commonly used?
    - The SparkFun MAX3010x Sensor Library is one of the most commonly used libraries because it simplifies reading heart-rate data from the sensor

### OLED Display (SSD1306)
 - Resolution: 128 × 64 pixels

 - I²C address: Most SSD1306 displays use the address 0x3C, although some modules can use 0x3D

 - SDA pin: A4 on the Arduino Nano

 - SCL pin: A5 on the Arduino Nano

### MicroSD Card Module
SPI pins:
 Nano Pin:      Function:
 D10            Chip Select (CS)
 D11            MOSI (Master Out Slave In)
 D12            MISO (Master In Slave Out)
 D13            SCK (Serial Clock)
Required libraries:
 - SD (built into the Arduino IDE)
 - SPI (built into the Arduino IDE)


### Breadboard w/ Jumper wires