# FIREGUARD AI — Hardware Schematic

This directory contains the circuit schematics and wiring documentation
for the FIREGUARD AI prototype.

## Initial Hardware Architecture

```text
              ┌──────────────────┐
              │      DHT22       │
              │ Temperature      │
              │ + Humidity       │
              └────────┬─────────┘
                       │
                       │
              ┌────────▼─────────┐
              │      ESP32       │
              │ Sensor Controller│
              └────────┬─────────┘
                       │
                  Wi-Fi / MQTT
                       │
                       ▼
              ┌──────────────────┐
              │ FIREGUARD Backend│
              └──────────────────┘


              ┌──────────────────┐
              │     Camera      │
              └────────┬─────────┘
                       │
                       ▼
              ┌──────────────────┐
              │  Raspberry Pi   │
              │    Edge AI      │
              └────────┬─────────┘
                       │
                       ▼
                 Risk Engine
                       │
                ┌──────┴──────┐
                ▼             ▼
             Buzzer          LED
