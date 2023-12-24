# Arduino Motion Detection with PIR Sensor

Welcome to the Arduino Motion Detection with PIR Sensor project repository! This repository contains multiple branches, each representing a different version of the Arduino code for motion detection using a Passive Infrared (PIR) sensor. Below, you'll find a comparison of the different versions available in this repository.

## Hardware Setup

### Components Required

- **Arduino Board:** Any Arduino board compatible with the Arduino IDE.
- **Passive Infrared (PIR) Sensor:** Detects motion and is connected to the Arduino board.
- **LED:** Used to indicate motion detection.

### Pin Connections

- **LED Pin (LED_pin):** Connect the positive leg of the LED to digital pin 13 and the negative leg through a current-limiting resistor to the ground (GND).
- **PIR Sensor Pin (PIR_INPUT):** Connect the signal pin of the PIR sensor to digital pin 2.

## Versions Comparison

### 1. `cpp-no-sleep` Branch

- **Functionality**:
  - Arduino code written entirely in C++ without utilizing sleep mode functionality.
  - Controls an LED based on motion detection from a PIR sensor.
  - Turns on the LED for a specific duration upon detecting motion.

- **Memory Usage**:
  - Program Storage Space: Uses 1050 bytes (3%) of program storage space.
  - Dynamic Memory (RAM): Global variables use 9 bytes (0%) of dynamic memory.

### 2. `cpp-with-sleep` Branch

- **Functionality**:
  - Arduino code written in C++ and includes sleep mode functionality.
  - Controls an LED based on motion detection from a PIR sensor.
  - Utilizes sleep mode to conserve power when not actively detecting motion.

- **Memory Usage**:
  - Program Storage Space: Uses 1204 bytes (3%) of program storage space.
  - Dynamic Memory (RAM): Global variables use 14 bytes (0%) of dynamic memory.

### 3. `cpp-register-writing-with-sleep` Branch

- **Functionality**:
  - Arduino code in C++ with direct MCU register writing and incorporates sleep mode functionality.
  - Controls an LED based on motion detection from a PIR sensor.
  - Employs direct register manipulation alongside sleep mode for advanced control and power efficiency.

- **Memory Usage**:
  - Program Storage Space: Utilizes 670 bytes (2%) of program storage space.
  - Dynamic Memory (RAM): Global variables use 10 bytes (0%) of dynamic memory.

<details>
  <summary><b>Authors</b></summary>

  This project uses the same hardware configuration across all versions and was authored by Itamar Meir. Contributions from the open-source community are welcome and encouraged.
</details>


