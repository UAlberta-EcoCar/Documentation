---
title: STM32 PCB Design
parent: PCB Design
nav_order: 1
---

EcoCar PCBs use STM32 Microcontrollers.

# Choosing a Microcontroller

I recommend starting with a STM32L432KC. 
If you took ECE-212, then you would have been given a NUCLEO-L432KC or similar.
A NUCLEO-L432KC is a development board with a STM32L432KC MCU. 
Which means you will be able to prototype your PCB using your development board.

If a STM32L432KC does not meet your design requirements, then you 
will need to pick a different MCU. 
Check the STM32 [website](https://www.st.com/en/microcontrollers-microprocessors/stm32-32-bit-arm-cortex-mcus.html) 
to see your options.

# How to design a STM32 MCU on a PCB

1. Go to the STM32 page of your MCU.

    Example: [STM32L432KC](https://www.st.com/en/microcontrollers-microprocessors/stm32l432kc.html#documentation)
1. Go to the Documentation section.
1. Search for `hardware development`
1. There should be a document called `Getting started with <STM32 MCU> Series hardware development`. 
Download it.
1. Go to the `Reference design` section in the document.
You should find an example of how to configure the MCU on a PCB.
I also recommend reading the `Recommendations` section of the document.

    Example: [STM32L432KC Reference Design](../../assets/an4555-getting-started-with-stm32l4-series-and-stm32l4-series-hardware-development-stmicroelectronics.pdf#page=49)
1. Copy the relevant parts of the reference design into your schematic.
