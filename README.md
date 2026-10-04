# FeroFlyF405
![FeroFlyF405.jpg](/FeroFlyF405.jpg)
FeroFlyF405 is an opensource flight controller based on STM32F405 and runs the open source flight controller firmware, [INAV](https://github.com/iNavFlight/inav).

FeroFlyF405 is designed to be an open hardware platform that enthusiasts and developers can study, modify, build, and use in their own projects.

## Features

* **Microcontroller:** STM32F405
* **IMU:** LSM6DSL 6-axis accelerometer and gyroscope
* **Barometer:** DPS368
* **Firmware:** INAV
* **Motor outputs:** 12 timer-based output channels
* **CAN bus:** For compatible peripherals
* **I2C:** External sensor and peripheral connectivity
* **UARTs:** 3 serial ports
* **PINIO:** 2 programmable GPIO outputs
* **Current sensing:** Dedicated input for an external current sensor

## Sponsor

A special thanks to **[NextPCB](https://www.nextpcb.com/)** for sponsoring the FeroFlyF405 project and supporting the development of this open-source flight controller.

Their support helped bring the custom PCB design from the screen to the physical board.

Thank you, NextPCB, for supporting open-source hardware development!

Get high quality PCBs for your project at an affordable rate from **[NextPCB](https://www.nextpcb.com/)**.

## Connectivity

| Interface      | Quantity | Purpose                                             |
| -------------- | -------: | --------------------------------------------------- |
| Motor outputs  |       12 | ESCs and other compatible timer-based outputs       |
| CAN bus        |        1 | Compatible CAN peripherals                          |
| I2C            |        1 | External sensors and peripherals                    |
| UART           |        3 | Receivers, GPS, telemetry, and other serial devices |
| PINIO          |        2 | User-configurable GPIO outputs                      |
| Current sensor |        1 | External current-sensing module                     |

> **Note:** Motor output capabilities depend on timer allocation, DMA availability, and firmware configuration. Not all outputs necessarily support every ESC protocol.

## Connectors and Pinout

FeroFlyF405 follows the **Pixhawk connector and pinout standard** for its applicable peripheral interfaces and uses **JST-GH series connectors**.

The PINIO and current-sensor connectors are exceptions to this convention.

## Firmware

FeroFlyF405 runs [INAV](https://github.com/iNavFlight/inav), an open-source flight control firmware for multirotor, fixed-wing, and other UAV platforms.

FeroFlyF405 uses a board-specific INAV target to configure its MCU pins, sensors, timers, communication interfaces, and other hardware resources.

Useful links:
* [FeroFlyF405 Target & Binary](https://github.com/Ozonised/FeroFlyF405-INAV-files)
* [INAV source code](https://github.com/iNavFlight/inav)
* [INAV documentation](https://inavflight.github.io/)

## 3D-Printed Enclosure

The FeroFlyF405 enclosure consists of three 3D-printable parts:

* **Enclosure Top** (`FeroFlyF405 Enclosure-Top.stl`) — Upper section of the enclosure.
* **Enclosure Bottom** (`FeroFlyF405 Enclosure-Bottom.stl`) — Lower section of the enclosure.
* **LED Cap** (`FeroFlyF405 Enclosure-Led Cap.stl`) — Cover for the status and power LEDs, designed to be printed using translucent filament to allow the LED light to pass through.

### Printing Recommendations

* **Top and Bottom:** PETG filament is recommended for durability and heat resistance.
* **LED Cap:** Use translucent filament for better LED visibility.
* **Fasteners:** The enclosure uses M3 screws and threaded inserts.

The STL files are provided so you can print and assemble the enclosure yourself.
