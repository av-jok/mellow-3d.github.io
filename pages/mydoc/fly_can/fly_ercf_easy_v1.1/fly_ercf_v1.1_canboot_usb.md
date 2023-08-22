---
title: Katapult Configuration for the Fly-ERCF-Easy-BRD-V1.1 on USB
tags: []
keywords: 
last_updated: 22/08/2023
summary: "How to Configure Katapult for USB Operation on the Fly-ERCF-Easy-BRD-V1.1"
sidebar: mydoc_sidebar
permalink: fly_ercf_v1.1_canboot_usb.html
folder: mydoc
comments: false
toc: true
datatable: true
boardname: Fly-ERCF-Easy-BRD-V1.1
firmware: USB
mcu: "rp2040"
version: v1
kconfig_name: ercfv1.1
architecture: "(Raspberry Pi RP2040)"
flash: "(W25Q080 with CLKDIV 2)"
deployment: "(Do not build)"
communication: "(USB)"
gpio_bootloader_set: "()"
support_bootloader_entry: "[*]"
enable_bootloader_gpio: "[&nbsp;]"
enable_status: "[*]"
status_pin: "(gpio17)"
board_type: "toolboard"
katapult_file: "katapult.uf2"

katapult_img1: "katapult/rp2040_usb_gpio17.png"
katapult_cap1: "Katapult Menu Config USB"

katapult_img2: "ercf_easy_v1.1/boot_button.png"
katapult_cap2: "Fly-ERCF-Easy-BRD-V1.1 Boot Button Location"

katapult_img3: "ercf_easy_v1.1/lsusb_screenshot.png"
katapult_cap3: "lsusb Results"

installKlipperURL: "./fly_ercf_v1.1_klipper_can.html"
installKlipperName: "Klipper for CANbus configuration section"

---
{% include important.html content="This guide assumes you have a working Klipper host installation on a Raspberry Pi or compatible device" %}

{% include custom/katapult/compile.html %}

{% include custom/katapult/rp2040_usb_flash.html %}

{% include custom/mcu/ercf_v1.1/ercf_v1.1_links.html %}