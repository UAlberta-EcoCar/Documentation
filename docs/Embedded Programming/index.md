---
title: STM32 Programming
nav_order: 4 
---

This section focuses on programming STM32 Microcontrollers.

### Table of Contents
{: .no_toc}

1. 
{:toc}

# Installation & Setup

1. Download and install [STM32CubeMX](https://www.st.com/en/development-tools/stm32cubemx.html).

    STM32CubeMX is an application for generating initialization code for STM32 MCUs.
    It also has a graphical interface for configuring the peripherals of a microcontroller.

1. Download a version of [STM32CubeIDE](https://www.st.com/content/st_com/en/stm32cubeide.html?tab=documentation#stm32-software-downloads-container). 

    STM32CubeIDE is an integrated development environment for writing and debugging code for STM32 microcontrollers.

    There are 2 versions to choose from: `STM32CubeIDE` (Eclipse IDE) and `STM32CubeIDE for VS Code` (VSCode Extension).
  
    `STM32CubeIDE for VS Code` is a VSCode extension and is more lightweight and flexible then its Eclipse based counterpart.
    However, it is still relatively new so most online tutorials will still be using `STM32CubeIDE`. 
    You can download both versions and try them both out if your unsure.

    To ensure cross compatibility between different IDE versions, make sure to select `CMake` as the toolchain/IDE when creating a new project in STM32CubeMX.

## STM32CubeIDE for VS Code

The full documentation for the VSCode STM32 extension is at [https://dev.st.com/stm32cube-docs/stm32cubeide-vscode/1.0.1/en/global_toc.html](https://dev.st.com/stm32cube-docs/stm32cubeide-vscode/1.0.1/en/global_toc.html)[^1].

The introductory video covers creating a new project, installing the extension, and debugging.

<iframe width="620" height="320" src="https://www.youtube.com/embed/aWMni01XGeI" 
    title="Get started with STM32Cube for VS Code: from installation to debugging" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
    referrerpolicy="strict-origin-when-cross-origin" allowfullscreen>
</iframe>

Here are some important sections in the documentation:

* [Installation Instructions](https://dev.st.com/stm32cube-docs/stm32cubeide-vscode/1.0.1/en/docs/markup/getting_started/installation.html)
* [Creating and Importing a Project](https://dev.st.com/stm32cube-docs/stm32cubeide-vscode/1.0.1/en/docs/markup/getting_started/first_project_creation.html)
* [Debugging](https://dev.st.com/stm32cube-docs/stm32cubeide-vscode/1.0.1/en/docs/markup/development/debug.html)
* If your new to VSCode then I recommend reading through the [Development Chapter](https://dev.st.com/stm32cube-docs/stm32cubeide-vscode/1.0.1/en/docs/markup/development/index.html) of the documentation.

# Getting Started with STM32

DigiKey has a [playlist](https://www.youtube.com/playlist?list=PLEBQazB0HUyRYuzfi4clXsKUSgorErmBv) on programming STM32 microcontrollers[^2].
Recommend at least watching:
* [Part 1: Introduction to STM32CubeIDE](https://www.youtube.com/watch?v=hyZS2p1tW-g&list=PLEBQazB0HUyRYuzfi4clXsKUSgorErmBv&index=1)
* [Part 3: FreeRTOS](https://www.youtube.com/watch?v=OPrcpbKNSjU&list=PLEBQazB0HUyRYuzfi4clXsKUSgorErmBv&index=3)

    [FreeRTOS](https://www.freertos.org/) is a real-time operating system for embedded systems and is used for running multiple chunks of code in parallel. Most EcoCar firmware
    uses FreeRTOS.

<iframe width="620" height="320" 
    src="https://www.youtube.com/embed/hyZS2p1tW-g?list=PLEBQazB0HUyRYuzfi4clXsKUSgorErmBv" 
    title="Getting Started with STM32 and Nucleo Part 1: Introduction to STM32CubeIDE and Blinky – Digi-Key" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
    referrerpolicy="strict-origin-when-cross-origin" 
    allowfullscreen>
</iframe>

----

  [^1]: [STM32CubeIDE for Visual Studio Code Documentation](https://dev.st.com/stm32cube-docs/stm32cubeide-vscode/1.0.1/en/global_toc.html)
  [^2]: [DigiKey - Getting Started with STM32 and Nucleo Tutorial](https://www.youtube.com/playlist?list=PLEBQazB0HUyRYuzfi4clXsKUSgorErmBv)
