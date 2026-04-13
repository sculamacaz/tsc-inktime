# InkTime

Author: Luca Mazilescu

## Pinout Table

| Pin | Signal | Direction | Peripheral | Description |
|-----|--------|-----------|------------|-------------|
| P0.02 | SPI_SCK | Output | E-Paper Display | SPI clock |
| P0.03 | SPI_MOSI | Output | E-Paper Display | SPI data out |
| P0.05 | EPD_CS | Output | E-Paper Display | Chip select |
| P0.06 | SDA | Bidir | Fuel Gauge, Charger, IMU, Haptics | Shared I2C data |
| P0.07 | SCL | Output | Fuel Gauge, Charger, IMU, Haptics | Shared I2C clock |
| P0.08 | IMU_INT1 | Input | IMU (BMA423) | Interrupt line 1 |
| P0.11 | PMIC_INT | Input | Charger (BQ25180) | Fault/status interrupt |
| P0.12 | HAPTIC_EN | Output | Haptics (DRV2605) | Driver enable |
| P0.13 | — | Input | Button 1 | User button |
| P0.14 | — | Input | Button 2 | User button |
| P0.15 | EPD_DC | Output | E-Paper Display | Data/command select |
| P0.16 | EPD_RST | Output | E-Paper Display | Display reset |
| P0.17 | EPD_BUSY | Input | E-Paper Display | Busy status |
| P0.18 | RESET | Input | — | System reset |
| P1.00 | SWO | Output | Debug (pad) | SWD trace output |
| P1.01 | — | Output | EPD power gate | EPD power control |
| P1.02 | — | Input | Button 3 | User button |
| P1.08 | IMU_INT2 | Input | IMU (BMA423) | Interrupt line 2 |
| P1.10 | ALERT | Input | Fuel Gauge (MAX17048) | UV/OV alert |
| D+ | D+ | Bidir | USB-C connector | USB data+ |
| D− | D- | Bidir | USB-C connector | USB data− |
| XL1/XL2 | — | — | 32.768 kHz crystal | Low-frequency clock |
| XC1/XC2 | — | — | 32 MHz crystal | High-frequency clock |
| SWDCLK | SWDCLK | Input | Debug (pad) | SWD clock |
| SWDIO | SWDIO | Bidir | Debug (pad) | SWD data |
| ANT | RF | Output | 2.4 GHz antenna | Wireless antenna feed |

## Block Diagram

<p align="center">
  <img src="./Assets/block_diagram.svg" alt="InkTime Block Diagram"/>
</p>
