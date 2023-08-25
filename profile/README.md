# Useful Links

- [Discord ![discord](https://img.shields.io/discord/824493524413710336.svg?logo=discord)](https://discord.gg/ShUWykk38X)
- [Coding Guidelines](https://github.com/ZigEmbeddedGroup/.github/blob/main/GUIDELINES.md)
- [Project Website](https://microzig.tech)
- [Project Wiki](https://wiki.microzig.tech)

# MicroZig

- [Main Repository](https://github.com/ZigEmbeddedGroup/microzig): Core of the MicroZig Framework
- [MicroZig Driver Framework](https://github.com/ZigEmbeddedGroup/microzig-driver-framework): Generic peripherial device drivers that can be used with MicroZig

# Chip Family Support Matrix

| Chip Family                                                                 | Support  | Compiles | `main()` | Registers | HAL | Abstractions | CI Status                                                                                                          |
| --------------------------------------------------------------------------- | -------- | -------- | -------- | --------- | --- | ------------ | ------------------------------------------------------------------------------------------------------------------ |
| [RasperryPi RP2040](https://github.com/ZigEmbeddedGroup/raspberrypi-rp2040) | Mature   | ✅        | ✅        | ✅         | 🛠   | 🧪            | ![Build](https://github.com/ZigEmbeddedGroup/raspberrypi-rp2040/actions/workflows/build.yml/badge.svg?branch=main) |
| [ST STM32](https://github.com/ZigEmbeddedGroup/stmicro-stm32)               | Degraded | ❌        | ❓        | ❓         | ❓   | ❓            |                                                                                                                    |
| [Microchip AVR](https://github.com/ZigEmbeddedGroup/microchip-atmega)       | Degraded | ❌        | ❓        | ❓         | ❓   | ❓            |                                                                                                                    |
| [Gigadevice GD32](https://github.com/ZigEmbeddedGroup/gigadevice-gd32)      | Degraded | ❌        | ❓        | ❓         | ❓   | ❓            |                                                                                                                    |
| [NXP LPC](https://github.com/ZigEmbeddedGroup/nxp-lpc)                      | Degraded | ❌        | ❓        | ❓         | ❓   | ❓            |                                                                                                                    |
| [Espressif ESP](https://github.com/ZigEmbeddedGroup/espressif-esp)          | Degraded | ✅        | 🛠        | 🛠         | ❓   | ❓            |                                                                                                                    |
| [Nordic NRF5x](https://github.com/ZigEmbeddedGroup/nordic-nrf5x)            | Degraded | ❌        | ❓        | ❓         | ❓   | ❓            |                                                                                                                    |

✅ Completed, 🛠 Work in Progress, 🧪 Experimental, ❌ Broken, ❓ Unknown

# Auxiliary Projects

## Tools

- [regz](https://github.com/ZigEmbeddedGroup/regz): SVD/ATDF to Zig converter 
- [zcom](https://github.com/ZigEmbeddedGroup/zcom): Cross-platform serial terminal emulator
- [uf2](https://github.com/ZigEmbeddedGroup/uf2): UF2 file generator

## Libraries

- [zfat](https://github.com/ZigEmbeddedGroup/zfat): FAT12/16/32 library
- [serial](https://github.com/ZigEmbeddedGroup/serial): Cross-platform serial port library for Windows, Linux, macOs, …

