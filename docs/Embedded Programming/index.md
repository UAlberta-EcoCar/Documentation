---
title: Embedded Programming 
nav_order: 4 
---

This section focuses on programming STM32 Microcontrollers.

### Table of Contents
{: .no_toc}

1. Getting Started
{:toc}

# Getting Started

1. Download and install [STM32CubeMX](https://www.st.com/en/development-tools/stm32cubemx.html).
STM32CubeMX is an application for generating initialization code for STM32 MCUs.
It also has a graphical interface for configuring the peripherals of a microcontroller.

1. Download a version of [STM32CubeIDE](https://www.st.com/content/st_com/en/stm32cubeide.html?tab=documentation#stm32-software-downloads-container)

    There are 2 versions to choose from: `STM32CubeIDE` and `STM32CubeIDE for VS Code`.
  
    I recommend `STM32CubeIDE for VS Code` over `STM32CubeIDE` for a few reasons:
    * Not based on Eclipse, more lightweight.
    * VSCode is a better code editor.
    * Access to VSCode extensions, git integration, copilot integration, etc.
    * Projects do not require a specific version of STM32CubeIDE to open unlike the eclipse counterpart.
    * Projects are compatible across multiple operating systems.

# STM32CubeIDE for VS Code

The full documentation for the VSCode STM32 extension is at [https://dev.st.com/stm32cube-docs/stm32cubeide-vscode/1.0.1/en/global_toc.html](https://dev.st.com/stm32cube-docs/stm32cubeide-vscode/1.0.1/en/global_toc.html).

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
* If your not experienced with using VSCode then I recommend reading through the [Development Chapter](https://dev.st.com/stm32cube-docs/stm32cubeide-vscode/1.0.1/en/docs/markup/development/index.html) of the documentation.
