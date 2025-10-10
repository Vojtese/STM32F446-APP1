# STM32F446-APP1

This repository contains the primary application slot for the STM32F446 dual-slot bootloader system. It is designed to work alongside the [STM32F446 Bootloader](https://github.com/Vojtese/STM32F446-Bootloader) and [STM32F446-APP2](https://github.com/Vojtese/STM32F446-APP2) as part of a robust firmware update architecture.

## 🚀 Features

- Application logic for Slot A
- Compatible with bootloader jump logic and SCB->VTOR relocation
- CRC integrity verification support
- UART communication interface
- STM32CubeIDE project structure

## 📁 Project Structure

- `Core/`: Application source files
- `Drivers/`: STM32 LL drivers
- `.ioc`: STM32CubeMX configuration file
- `STM32F446RETX_FLASH.ld`: Linker script aligned with bootloader memory map

## 🔗 Related Repositories

- [STM32F446-Bootloader](https://github.com/Vojtese/STM32F446-Bootloader)
- [STM32F446-APP2](https://github.com/Vojtese/STM32F446-APP2)

## 📜 License

This project is licensed under the GNU General Public License v3.0.
