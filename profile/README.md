# Useful Links

- [Discord ![discord](https://img.shields.io/discord/824493524413710336.svg?logo=discord)](https://discord.gg/ShUWykk38X)
- [Coding Guidelines](https://github.com/ZigEmbeddedGroup/.github/blob/main/GUIDELINES.md)
- [Project Website](https://microzig.tech)
- [Project Wiki](https://wiki.microzig.tech)

# MicroZig

- [Main Repository](https://github.com/ZigEmbeddedGroup/microzig): Core of the MicroZig Framework
- [MicroZig Examples](https://github.com/ZigEmbeddedGroup/microzig-examples): Contains usage examples for all board support packages
- [MicroZig Driver Framework](https://github.com/ZigEmbeddedGroup/microzig-driver-framework): Generic peripherial device drivers that can be used with MicroZig

# Chip Family Support Matrix

| Chip Family                                                                 | Support  | Examples                                                                                       | Compiles | `main()` | Registers | HAL | Abstractions | CI Status |
| --------------------------------------------------------------------------- | -------- | ---------------------------------------------------------------------------------------------- | -------- | -------- | --------- | --- | ------------ | --------- |
| [RasperryPi RP2040](https://github.com/ZigEmbeddedGroup/raspberrypi-rp2040) | Mature   | [Examples](https://github.com/ZigEmbeddedGroup/microzig-examples/tree/main/raspberrypi-rp2040) | ✅        | ✅        | ✅         | 🛠   | 🧪            | *Missing* |
| [ST STM32](https://github.com/ZigEmbeddedGroup/stmicro-stm32)               | Rough    | [Examples](https://github.com/ZigEmbeddedGroup/microzig-examples/tree/main/stmicro-stm32)      | ✅        | ❓        | ❓         | ❓   | ❓            | *Missing* |
| [Microchip AVR](https://github.com/ZigEmbeddedGroup/microchip-atmega)       | Degraded | [Examples](https://github.com/ZigEmbeddedGroup/microzig-examples/tree/main/microchip-atmega)   | ❌        | ❓        | ❓         | ❓   | ❓            | *Missing* |
| [Gigadevice GD32](https://github.com/ZigEmbeddedGroup/gigadevice-gd32)      | Degraded | [Examples](https://github.com/ZigEmbeddedGroup/microzig-examples/tree/main/gigadevice-gd32)    | ✅        | ❓        | ❓         | ❓   | ❓            | *Missing* |
| [NXP LPC](https://github.com/ZigEmbeddedGroup/nxp-lpc)                      | Rough    | [Examples](https://github.com/ZigEmbeddedGroup/microzig-examples/tree/main/nxp-lpc)            | ✅        | ❓        | ❓         | ❓   | ❓            | *Missing* |
| [Espressif ESP](https://github.com/ZigEmbeddedGroup/espressif-esp)          | Rough    | [Examples](https://github.com/ZigEmbeddedGroup/microzig-examples/tree/main/espressif-esp)      | ✅        | 🛠        | 🛠         | ❓   | ❓            | *Missing* |
| [Nordic NRF5x](https://github.com/ZigEmbeddedGroup/nordic-nrf5x)            | Rough    | [Examples](https://github.com/ZigEmbeddedGroup/microzig-examples/tree/main/nordic-nrf5x)       | ✅        | 🛠        | 🛠         | ❓   | ❓            | *Missing* |

✅ Completed, 🛠 Work in Progress, 🧪 Experimental, ❌ Broken, ❓ Unknown

# Auxiliary Projects

## Tools

- [regz](https://github.com/ZigEmbeddedGroup/regz): SVD/ATDF to Zig converter 
- [zcom](https://github.com/ZigEmbeddedGroup/zcom): Cross-platform serial terminal emulator
- [uf2](https://github.com/ZigEmbeddedGroup/uf2): UF2 file generator

## Libraries

- [zfat](https://github.com/ZigEmbeddedGroup/zfat): FAT12/16/32 library
- [serial](https://github.com/ZigEmbeddedGroup/serial): Cross-platform serial port library for Windows, Linux, macOs, …

