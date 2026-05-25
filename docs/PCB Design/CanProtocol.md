---
title: CAN Protocol
parent: PCB Design
nav_order: 2 
---

EcoCar uses the [CAN protocol](https://www.csselectronics.com/pages/can-bus-simple-intro-tutorial) to communicate between PCBs.
CAN is a standard communication protocol used in vehicles, offering high speed and reliability.
A [CAN transceiver](https://www.infineon.com/knowledge-centre/what-is-a-can-transceiver) is required for communication
between multiple MCUs. Currently we use a [MCP2542FD](https://www.microchip.com/en-us/product/MCP2542FD) for the CAN transceiver.

There are multiple ways to configure CAN on an MCU. 
Currently we use either CAN 2.0 or CAN FD with a **fixed** baud rate of `1 Mbit/s`.

To connect PCBs together, most EcoCar PCBs have a DSUB 7W2 Connector.

Communication between multiple MCUs requires each MCU to interpret CAN data in the same way.
That is why in the EcoLib library there is a [ecocan](https://github.com/UAlberta-EcoCar/EcoLib/tree/main/ecocan) folder
containing files to include in your firmware. These files are needed to setup CAN on the firmware side.
