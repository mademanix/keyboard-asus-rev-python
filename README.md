# Reverse Engineering Asus Rog Azoth USB Communication

## Overview

This project aims to reverse engineer the USB communication of the Asus Rog Azoth keyboard to create a Python script for controlling lighting, key mapping, and other features without relying on the Asus Armoury Crate app.

## Goals
- Understand the USB protocol used by Asus Rog Azoth.
- Develop a Python script to change lighting and key mapping.
- Enable control over the keyboard's features independent of official software.

## Requirements
- Asus Rog Azoth keyboard.
- Wireshark (with USBPcap for packet capture).
- PyUSB or libusb for USB communication in Python.

## Steps
- Capture USB traffic using Wireshark while interacting with the keyboard.
- Analyze the captured packets to decode key mappings, lighting controls, etc.
- Write a Python script using PyUSB to send commands to the keyboard.

## Useful links and docs
- https://www.elprocus.com/usb-protocol/

## License
TBD — License choice depends on legal implications of reverse engineering. Please research thoroughly before contributing.