---

title: Fly-SB2040-V1 General Information
tags: []
keywords: 
last_updated: 23/07/2023
summary: "General information regarding the Fly-SB2040-V1"
sidebar: mydoc_sidebar
permalink: fly_sb2040_v1_general.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-SB2040-V1
firmware: CAN bus
version: v1

overview_img1: "fly-sb2040_v1/sb2040.png"
overview_cap1: "Fly-SB2040-V1 Front and Rear view"

overview_img2: "fly-sb2040_v1/sb2040_size.jpg"
overview_cap2: "Fly-SB2040-V1 dimensions"

overview_img3: "fly-sb2040_v1/sb2040_bom.png"
overview_cap3: "Fly-SB2040-V1 BOM"

---
## {{ page.boardname }} Overview

    {% capture mcustep %}{{ page.mcustep }}{% endcapture %}
    {% capture mcustep2 %}{{ page.mcustep2 }}{% endcapture %}
    {% capture mcusch %}{{ page.mcusch }}{% endcapture %}

    {% capture overurl1 %}.\images\{{page.overview_img1}}{% endcapture %}
    {% capture overurl2 %}.\images\{{page.overview_img2}}{% endcapture %}       
    {% capture overurl3 %}.\images\{{page.overview_img3}}{% endcapture %}   

### Description

The {{page.boardname}} toolboard uses CAN communication to connect the host computer with a UTOC board, other USB to CAN adapters, Pi Hats, USB to CAN Bridge Mode in Klipper or USB. For USB use it is recommended to not to use a cable that exceeds 1 meter ( 3.2 feet ) in length.  
The {{page.boardname}} can no longer be purchased through AliExpress as it has been replaced by the Fly-SB2040-V2

{% include image.html file=page.overview_img1 url=overurl1 alt=page.overview_cap1 caption=page.overview_cap1 %}

### Product Features

- CANbus connection for stable data transmission over long distaces.
- 24 volt max input
- 5 amp mosfet for heater control
- Onboard TMC2209 driver for the extruder
- Onboard ADXL345 accelerometer to measure resonance for input shaper.
- 3 controllable fans.
- RGB Led control
- Peripheral interface:USB*1, CAN*1, FAN*3, RGB*1, Servo*1, Probe*1, EndStop*3, Thermal*1, Heater*1

{% include image.html file=page.overview_img2 url=overurl2 alt=page.overview_cap2 caption=page.overview_cap2 %}

### BOM

{% include image.html file=page.overview_img3 url=overurl3 alt=page.overview_cap3 caption=page.overview_cap3 %}

### Included parts

- {{ page.boardname }} Board
- Heatsink for 2209 driver
- Jumpers * 2
- JST-PH plugs and Female Crimp Terminals
- Microft plug and Crimp Terminals
- XT30+2 1 meter 4 wire harness
- USB-A to USB-C Cable

{% include custom/mcu/sb2040v1/sb2040_v1_links.html %}