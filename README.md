# STM32F446 Application Slot 1 (APP1)

This repository contains the primary application firmware for the STM32F446-based signal acquisition unit, developed as part of a rainwater retention system. The firmware is designed to acquire, process, and transmit sensor data from an underground tank to a central unit via RS-485.

## 🚀 Features

- Acquisition of analog and digital sensor data:
  - Pressure (piezoresistive)
  - Flow (turbine and differential)
  - Temperature (1-Wire DS18B20)
  - Voltage and current sensing
- Signal conditioning and filtering
- RS-485 communication using UART + DMA
- Application logic structured around state machines
- Compatible with bootloader jump logic and memory partitioning
- CRC validation and watchdog integration (optional)

## 🧠 CMSIS LL Driver Usage

- `LL_ADC_REG_StartConversion()`, `LL_ADC_REG_ReadConversionData32()` – ADC sampling
- `LL_USART_TransmitData8()`, `LL_USART_IsActiveFlag_TXE()` – UART transmission
- `LL_DMA_EnableChannel()` – DMA for UART
- `LL_GPIO_IsInputPinSet()` – digital sensor polling

## 📁 Project Structure

- `Core/`: Application logic and sensor routines
- `Drivers/`: STM32 LL drivers
- `.ioc`: STM32CubeMX configuration
- `STM32F446RETX_FLASH.ld`: Linker script for App1 memory region

## 🔗 Related Projects

- [STM32F446-Bootloader](https://github.com/Vojtese/STM32F446-Bootloader)
- [STM32F446-APP2](https://github.com/Vojtese/STM32F446-APP2)
- [STM32F446-SensorTestAndHW](https://github.com/Vojtese/STM32F446-SensorTestAndHW)

## 📜 License

This project is licensed under the GNU General Public License v3.0.
