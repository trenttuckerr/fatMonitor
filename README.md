# Fat Monitor Project

## Overview

This project combines assembly and C++ code to create a Fat Monitor system using an Arduino platform. The project involves both hardware and software components to read user input and control an LED display based on specified conditions.

## Repository Structure

- **`FatMonitor.S`**: Assembly code file responsible for implementing the core functionality of the Fat Monitor.
- **`FatMonitor.ino`**: Arduino sketch written in C++ that interfaces with the assembly code and sets up the system.

## Assembly Code (`FatMonitor.S`)

The assembly code defines the core logic for the Fat Monitor. It includes functionality to light up LEDs based on user input, distinguishing between different gender and age categories. The assembly code is integrated with the Arduino sketch using the `extern "C"` block.

## Arduino Sketch (`FatMonitor.ino`)

The Arduino sketch initializes serial communication, reads user input for gender, age, and fat values, and then calls the assembly code (`fatmonitor()`) to control the LED display. The project involves a delay loop in the `loop()` function for periodic LED blinking.

## Getting Started

1. Connect the Arduino platform to the necessary hardware components.
2. Upload the `FatMonitor.ino` sketch to the Arduino board.
3. Monitor the serial output to interactively input gender, age, and fat values.

## Notes

- The `lightup()` function lights up all LEDs, useful for initial testing.
- The LED display color and pattern are determined based on gender, age, and fat values.
- The `read2DigitHexValue()` function allows users to input values in hexadecimal format.

## Dependencies

- Arduino IDE (or compatible development environment).
- Arduino board compatible with the code.

## Author

- Trent Tucker

