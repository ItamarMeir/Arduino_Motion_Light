# Motion-Activated LED Control using Arduino

This Arduino sketch controls an LED based on motion detection from a Passive Infrared (PIR) sensor. When motion is detected, the LED connected to digital pin 13 (LED_pin) will turn on for a specific duration before turning off.

## Hardware Setup
- **LED_pin (digital pin 13):** Connect an LED's positive leg (longer lead) to this pin and the negative leg (shorter lead) to ground through a current-limiting resistor.
- **PIR_INPUT (digital pin 2):** Connect the signal pin of a PIR motion sensor to this pin.

## Code Overview
- **Constants:** Define pin assignments and delay time for the LED.
- **Setup Function:**
  - Configure pin modes for the LED and PIR sensor.
- **Loop Function:**
  - Read the value from the PIR sensor.
  - If motion is detected, turn on the LED for a specific time before turning it off.

## Memory Usage
- **Program Storage Space:** This sketch uses 1050 bytes (3%) of program storage space, with a maximum of 32256 bytes available.
- **Dynamic Memory (RAM):** Global variables use 9 bytes (0%) of dynamic memory, leaving 2039 bytes for local variables. The maximum available dynamic memory is 2048 bytes.

## How to Use
1. Connect the components based on the specified pin configurations.
2. Upload the sketch to your Arduino board.
3. Observe the LED behavior: it will turn on upon detecting motion and turn off after the specified delay.

## Additional Notes
- Ensure the correct pin connections and component configurations for proper functionality.

## Author
This code was authored by Itamar Meir and can be modified or used according to your project requirements.
