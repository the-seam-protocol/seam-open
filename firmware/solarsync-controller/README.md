# SolarSync Controller Firmware

> MPPT charge controller + BMS + PAYGo logic for the SolarSync citizen node.

## Target Platform
- **MCU**: STM32L4 series (low power) or ESP32-S3
- **Language**: C17 (STM32 HAL) or Rust

## Features
- [ ] MPPT algorithm (Perturb & Observe + Incremental Conductance)
- [ ] 16S LFP cell balancing (passive)
- [ ] Per-cell voltage and temperature monitoring
- [ ] PAYGo token validation (prepaid energy credits)
- [ ] LoRa telemetry uplink (energy production, consumption, battery SOC)
- [ ] Over-the-air (OTA) firmware updates via LoRa

## Status
🔴 **Not started**
