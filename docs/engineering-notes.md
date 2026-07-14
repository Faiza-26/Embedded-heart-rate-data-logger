# July 15, 2026
## Objective
Connect the MAX30102 pulse oximeter to the Arduino Nano and verify I²C communication.
---
## Hardware Used
- Arduino Nano V3
- MAX30102 (HW-605) Pulse Oximeter
- Breadboard
- Jumper Wires
---
## Wiring
VIN  → 5V
GND → GND
SDA → A4
SCL → A5
---
## Progress
- Successfully wired the MAX30102.
- Uploaded the SparkFun Basic Readings example.
- The sensor initially could not be detected.
- Used an I²C scanner to diagnose the issue.
- Initially received:
    No I2C devices found.
- After improving the mechanical connection between the sensor and breadboard:
    I2C device found at address 0x57
- Successfully confirmed communication with the sensor.
---
## Problems Encountered
The sensor made inconsistent contact with the breadboard.
---
## Solution
Pressed the breakout board firmly into the breadboard and verified communication using an I²C scanner before testing higher-level code.
---
## Lessons Learned
Debug hardware one layer at a time.
1. Verify power.
2. Verify communication.
3. Verify software.
4. Verify functionality.
The I²C scanner is one of the most useful debugging tools for embedded systems.
---
## Next Session
- Improve sensor contact.
- Run HeartRate example.
- Measure BPM.
- Understand signal quality.