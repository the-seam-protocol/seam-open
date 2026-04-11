# SolarSync — Citizen Node

> The foundational energy unit for every Sudanese household.

## Specifications

| Parameter | Value |
|-----------|-------|
| Solar Array | 5 kW (Tier-1 PV, >22% efficiency) |
| Battery | 10 kWh LFP (3.2V cells, 16S configuration) |
| Water Generation | AWG 20–30 L/day |
| Connectivity | LoRaWAN 868/915 MHz (15 km LOS) |
| Payment Model | PAYGo (zero upfront) |
| Operating Temp | -10°C to +70°C |
| Enclosure | IP65, UV-stabilized |

## Block Diagram

```
Solar Panels (5kW)
       │
       ▼
┌──────────────┐    ┌──────────────┐
│ MPPT Charge  │───▶│ LFP Battery  │
│ Controller   │    │ Pack (10kWh) │
└──────┬───────┘    └──────┬───────┘
       │                   │
       ▼                   ▼
┌──────────────┐    ┌──────────────┐
│ DC Bus       │───▶│ Inverter     │──▶ AC Output (240V)
│ Distribution │    │ (Pure Sine)  │
└──────┬───────┘    └──────────────┘
       │
       ├──▶ AWG Unit (atmospheric water generator)
       ├──▶ LoRa Gateway (telemetry + mesh)
       └──▶ Soil Sensor Array (optional, Phase 3 prep)
```

## Directory Structure

```
solarsync/
├── pcb/                  # KiCad projects
│   ├── mppt-controller/  # MPPT charge controller board
│   ├── bms-16s/          # 16S LFP battery management board
│   ├── inverter/         # DC-AC inverter control board
│   └── sensor-hub/       # LoRa + sensor interface board
├── mechanical/           # FreeCAD models
│   ├── enclosure/        # IP65 outdoor enclosure
│   ├── mounting/         # Panel mounting brackets
│   └── battery-rack/     # LFP cell rack assembly
├── bom/                  # Bill of Materials (CSV)
└── README.md             # This file
```

## Status

🔴 **Not started** — Seeking KiCad contributors for MPPT controller schematic.
