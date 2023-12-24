# Motion-Activated LED Control using Arduino

This Arduino sketch controls an LED based on motion detection from a Passive Infrared (PIR) sensor. When motion is detected, the LED connected to pin 13 (PORT B) will turn on for a specific duration before turning off.

## Hardware Setup
- **LED_pin (pin 13):** Connect an LED's positive leg (longer lead) to this pin and the negative leg (shorter lead) to ground through a current-limiting resistor.
- **PIR_INPUT (pin 2):** Connect the signal pin of a PIR motion sensor to this pin.

## Code Overview
- **Constants:** Define pin assignments and delay time for the LED.
- **Setup Function:**
  - Configure pin modes for the LED and PIR sensor.
  - Set the sleep mode for power-saving purposes.
  - Enable an external interrupt on the PIR sensor pin for motion detection.
- **Loop Function:**
  - Disable sleep mode to operate normally.
  - Check for motion detection.
  - If motion is detected, turn on the LED for a specific time before turning it off.
  - Enter sleep mode to save power when no motion is detected.
- **Interrupt Service Routine (ISR):** When the external interrupt occurs (INT0), it sets the motion detection flag.

## Memory Usage
- **Program Storage Space:** This sketch uses 670 bytes (2%) of program storage space, with a maximum of 32256 bytes available.
- **Dynamic Memory (RAM):** Global variables use 10 bytes (0%) of dynamic memory, leaving 2038 bytes for local variables. The maximum available dynamic memory is 2048 bytes.

## How to Use
1. Connect the components based on the pin configurations specified.
2. Upload the sketch to your Arduino board.
3. Observe the LED behavior: it will turn on upon detecting motion and turn off after the specified delay.

## Additional Notes
- The code utilizes sleep mode to reduce power consumption when there is no motion detected, conserving energy.
- Ensure the correct pin connections and component configurations for proper functionality.

## Author
This code was authored by [Your Name or Username] and can be modified or used according to your project requirements.
