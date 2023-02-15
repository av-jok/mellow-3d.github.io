---
title: Fly-E3 v2 Klipper firmware in USB to Can Bridge
tags: []
keywords: 
last_updated: 20/10/2022
summary: "Fly-E3 v2 Klipper USB to CAN"
sidebar: mydoc_sidebar
permalink: fly-e3_v2_klipper_usbtocan.html
folder: mydoc
comments: false
toc: true
datatable: true


boardname: Fly-E3 v2
firmware: usbtocan
version: v1
processor: "STM32F407"
offset: "32 KiB bootloader"
clock: "8 MHz crystal"

com: "USB to CAN Bridge on PA11/PA12"


klipcom_img1: "fly-super8/fly-super8_klipper_menuconfig_usb_can_bridge.png"
klipcom_cap1: "Klipper Menu Config USB to CAN"

klipcom_img2: "fly-super8/fly-super8_klipper_usb_burn.png"
klipcom_cap2: "Burn Klipper firmware over USB"

klipcom_img3: "fly-super8/flash-can_query.png"
klipcom_cap3: "Flash Can Query"


---

## Configuring and installing Klipper for USB to CAN bridge mode


{% include note.html content="If you are planning to use CANBoot bootloader with Klipper in USB to CAN bridge mode you will want to configure [CanBoot in USB mode](./fly-super8_canboot_usb.html)" %}

{% include custom/mcu/stm32/stm32_klipper_menuconfig.html %}

{% include custom/mcu/stm32/stm32_klipper_flash_canboot.html %}

{% include custom/can/sht_links.html %}