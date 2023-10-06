# Arduino Motion Detection with PIR Sensor

Welcome to the Arduino Motion Detection with PIR Sensor project repository! This repository contains multiple branches, each representing a different version of the Arduino code for motion detection using a Passive Infrared (PIR) sensor. Below, you'll find an explanation of each branch and its purpose.

## Branches

### 1. `main` Branch

- **Description**: The `main` branch serves as the default branch for this repository and contains important project documentation and information.
  
- **Contents**:
  - README: Project introduction, setup instructions, and usage guidelines.
  - CONTRIBUTING.md: Guidelines for contributing to this project.
  - LICENSE: Information about the project's license.

### 2. `cpp-no-sleep` Branch

- **Description**: The `cpp-no-sleep` branch contains the Arduino code written entirely in C++ without using sleep mode.
  
- **Purpose**: This branch showcases motion detection code without utilizing sleep mode for power-saving purposes.

### 3. `cpp-with-sleep` Branch

- **Description**: The `cpp-with-sleep` branch contains the Arduino code written entirely in C++ and includes sleep mode functionality.
  
- **Purpose**: This branch demonstrates motion detection code that utilizes sleep mode to conserve power when not actively detecting motion.

### 4. `cpp-register-writing-with-sleep` Branch

- **Description**: The `cpp-register-writing-with-sleep` branch includes code that uses C++ along with direct MCU register writing, and it also incorporates sleep mode functionality.
  
- **Purpose**: This branch explores motion detection code that employs direct register manipulation alongside sleep mode for advanced control and power efficiency.

## Getting Started

To get started with a specific branch, follow these steps:

1. Clone or fork this repository to your local development environment.
2. Switch to the desired branch using Git. For example, to switch to the `cpp-no-sleep` branch, use the command:
