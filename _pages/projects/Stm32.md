---
title: "Custom Stm32f103 Development Board"
layout: categories
permalink: /stm32/
collection: categories
entries_layout: grid
classes: wide
date: 2020-11-07T18:38:52+00:00

excerpt: "I created and designed a custom stm32 microcontroller development board."
header:
  teaser: /assets/img/pcp_small.jpg
sidebar:
  - title: "Stm32 Dev board"
    text: "Designer, Schematic and PCB design using kicad and Altium"
    
gallery:
  - url: /assets/img/igvc_pcb_1.png
    image_path: /assets/img/igvc_pcb_1.png
    alt: "Generic Dev Board"
  - url: /assets/img/Igvc_pcb_2a.JPG
    image_path: /assets/img/Igvc_pcb_2a.JPG
    alt: "Motor control board v2"
  - url: /assets/img/igvc_pcb_3.png
    image_path: /assets/img/igvc_pcb_3.png
    alt: "Motor control board v1" 
  - url: /assets/img/PCB.JPG
    image_path: /assets/img/pcp_small.jpg
    alt: "PCB Altium"
---

[Github Repo](https://github.com/TylerJulian/STM32F103RCT6-Dev-Board)

I designed a PCB with a STM32F103rct6 microcontroller that has ports for motor control, encoders, and CAN-Bus protocol. I wrote firmware to control the CAN-bus, PWM, Interupt, and GPIO pins. A PID is implemented using software to control the speed of the motors. The board is programmed using SWD. Each board has a CAN-bus transceiver.

There are two variations of the board. A generic development board and the motor controller board described above.

{% include gallery caption="Here are some examples of the soldered boards that I have designed for the stm32f103 MCU" %}