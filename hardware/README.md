# FIREGUARD AI Hardware

This directory contains the hardware components, firmware, circuit
schematics, and hardware documentation for FIREGUARD AI.

## Planned Hardware

- ESP32
- Raspberry Pi
- Camera
- DHT22 temperature and humidity sensor
- Smoke/gas sensor
- LED indicator
- Buzzer
- Breadboard and jumper wires

## Hardware Architecture

```text
Sensors
   ↓
ESP32
   ↓
Wi-Fi / MQTT
   ↓
FIREGUARD AI Backend
