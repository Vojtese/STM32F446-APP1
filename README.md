# STM32F446 Application Slot 1 (APP1)

This repository contains the primary application firmware for the STM32F446-based signal acquisition unit. It interfaces with sensors, performs diagnostics, and communicates with the central unit via RS485.

## 🚀 Features

- Sensor acquisition via ADC (pressure, flow, temperature)
- RS485 communication using UART + DMA
- Signal conditioning and filtering
- Compatible with bootloader jump logic
- CMSIS LL drivers for precise peripheral control

## 📁 Project Structure

- `Core/`: Application logic
- `Drivers/`: STM32 LL drivers
- `.ioc`: STM32CubeMX configuration
- `STM32F446RETX_FLASH.ld`: Linker script for App1 memory region

## 🔗 Related Projects

- [STM32F446-Bootloader](https://github.com/Vojtese/STM32F446-Bootloader)
- [STM32F446-APP2](https://github.com/Vojtese/STM32F446-APP2)

## 📜 License

This project is licensed under the GNU General Public License v3.0.
