# Sensor-Based Data Logger (STM32 + BME280 + SD Card)

## Overview

This project implements a **sensor-based data logger** using an STM32 microcontroller, a BME280 environmental sensor, and an SD card for data storage. The system is developed with **bare-metal embedded C**, utilizing **I2C and SPI communication protocols**, ADC functionality, and power budgeting techniques to ensure long-term battery operation.

## Features

- Reads temperature, humidity, and pressure data from the BME280 sensor via **I2C**.
- Logs sensor data to an SD card using the **SPI** interface.
- Utilizes ADC for additional analog sensor inputs (if any).
- Implements power management strategies for low power consumption.
- Designed to operate continuously for **weeks on battery power** without maintenance.

## Hardware Components

- STM32 Microcontroller (e.g., STM32F103C8)
- BME280 Sensor (temperature, humidity, pressure)
- SD Card Module
- Battery power supply

## Software

- Written in bare-metal C (no RTOS)
- Drivers for I2C, SPI, ADC peripherals
- File system handling for SD card data logging
- Power budgeting implemented via low-power modes and efficient sampling

## Usage

1. Build and flash the firmware onto the STM32 board.
2. Connect the BME280 sensor and SD card module as per the schematic.
3. Power the device with a suitable battery.
4. The system will automatically log sensor data at configured intervals.
5. Data can be retrieved from the SD card for analysis.

## Outcome

A robust embedded system capable of reliably logging environmental data over extended periods while optimizing power consumption.

---

## Personal Note

This project is part of my journey towards becoming a skilled embedded systems engineer. It helps me build foundational expertise in bare-metal programming, sensor interfacing, and low-power design, which are essential skills for developing reliable IoT and data acquisition systems.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
