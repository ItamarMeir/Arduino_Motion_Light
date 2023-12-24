# Motion-Activated LED Control with Sleep Mode using Arduino

This Arduino sketch controls an LED based on motion detection from a Passive Infrared (PIR) sensor. When motion is detected, the LED connected to digital pin 13 (LED_pin) will turn on for a specific duration before turning off. Additionally, the code utilizes sleep mode to conserve power when there's no motion detected.

## Hardware Setup
- **LED_pin (digital pin 13):** Connect an LED's positive leg (longer lead) to this pin and the negative leg (shorter lead) to ground through a current-limiting resistor.
- **PIR_INPUT (digital pin 2):** Connect the signal pin of a PIR motion sensor to this pin.

## Code Overview
- **Constants:** Define pin assignments and delay time for the LED.
- **Setup Function:**
  - Configure pin modes for the LED and PIR sensor.
  - Attach an interrupt to the PIR sensor pin for motion detection.
- **Loop Function:**
  - Check for motion detection.
  - If motion is detected, turn on the LED for a specific time before turning it off.
  - Enter sleep mode to save power when no motion is detected.
- **Interrupt Service Routine (ISR):** Sets the motion detection flag when the interrupt occurs.

## Memory Usage
- **Program Storage Space:** This sketch uses 1204 bytes (3%) of program storage space, with a maximum of 32256 bytes available.
- **Dynamic Memory (RAM):** Global variables use 14 bytes (0%) of dynamic memory, leaving 2034 bytes for local variables. The maximum available dynamic memory is 2048 bytes.

## How to Use
1. Connect the components based on the specified pin configurations.
2. Upload the sketch to your Arduino board.
3. Observe the LED behavior: it will turn on upon detecting motion and turn off after the specified delay. Sleep mode will be activated when no motion is detected, conserving power.

## Additional Notes
- The code implements sleep mode to reduce power consumption during periods without motion detection, enhancing energy efficiency.
- Ensure correct pin connections and component configurations for proper functionality.

## Author
This code was authored by Itamar Meir and can be modified or used according to your project requirements.
