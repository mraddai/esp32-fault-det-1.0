# esp32-fault-det-1.0
ESP32-based low-cost fault-detection node with on-device RMS computation, anomaly flags, and serial logging
# Low-Cost Embedded Fault-Detection Node (ESP32)

This project implements a low-cost embedded fault-detection node using an ESP32
and isolated voltage/current sensors.

## Features

- Samples voltage and current at 2 kHz using the ESP32 ADC.
- Computes RMS values on-device over a configurable sliding window.
- Detects over-voltage and over-current faults and drives an on-board LED.
- Streams JSON-formatted logs over the serial port for offline analysis.

## Tech Stack

- C++ firmware on ESP32 using PlatformIO and the Arduino framework.
- Optional Python tooling for log parsing and visualization.

## Getting Started

```bash
pip install platformio
cd firmware
pio run
pio upload
pio device monitor
