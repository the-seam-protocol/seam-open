# S.E.A.M Open Hardware & Software

**Sudanese Energy, Agriculture, and Mobility — Open Protocol**

> An open-source blueprint for building decentralized energy, mobility, and agriculture infrastructure in Sudan. This repository contains hardware designs, firmware, and software for every system described in the S.E.A.M Protocol.

[![License: CERN-OHL-P-2.0](https://img.shields.io/badge/Hardware-CERN--OHL--P--2.0-brightgreen)](https://ohwr.org/cernohl)
[![License: Apache-2.0](https://img.shields.io/badge/Software-Apache--2.0-blue)](https://www.apache.org/licenses/LICENSE-2.0)

---

## 🏗️ Repository Structure

```
seam-open/
├── hardware/                    # Hardware designs (KiCad, mechanical CAD)
│   ├── solarsync/               # SolarSync — Citizen Node (5kW PV + 10kWh LFP)
│   ├── officesync/              # OfficeSync — Commercial Hub (20–50kW)
│   ├── sfres/                   # SFRES — Industrial Pillar (250+kW)
│   ├── pulsetrike/              # PulseTrike — EV Rickshaw Conversion
│   ├── pulsevan/                # PulseVan — Light Logistics EV
│   ├── pulsebus/                # PulseBus — Mass Transit EV
│   ├── skateboard-chassis/      # Universal EV Skateboard Platform
│   ├── lora-gateway/            # LoRa Ghost Network Gateway
│   ├── battery-swap-module/     # Standardized Battery Swap Mechanism
│   └── swarm-robotics/          # Agricultural Swarm (Mother-Tractor, Pulse-Rover, Aero-Sentinel)
│
├── firmware/                    # Embedded firmware (C/Rust)
│   ├── solarsync-controller/    # MPPT + BMS + PAYGo controller
│   ├── lora-node/               # LoRaWAN node firmware (868/915 MHz)
│   ├── lora-gateway/            # Gateway coordinator firmware
│   ├── bms/                     # Battery Management System (LFP cells)
│   ├── battery-swap/            # Swap station controller
│   ├── e-axle-controller/       # Axial flux motor controller
│   └── swarm-autopilot/         # Swarm navigation (Mother-Tractor + Rovers)
│
├── software/                    # Server-side & application software
│   ├── mesh-id/                 # Mesh-ID identity system
│   ├── paygo-engine/            # PAYGo billing & smart contracts
│   ├── v2g-orchestrator/        # Vehicle-to-Grid energy trading
│   ├── soil-dna-platform/       # Soil mapping & polyculture AI
│   ├── faas-coordinator/        # Farming-as-a-Service orchestration
│   ├── ubi-ledger/              # Universal Basic Income distribution
│   ├── esg-certifier/           # ESG certificate issuance & verification
│   └── telemetry-dashboard/     # Real-time fleet & grid monitoring
│
├── manufacturing/               # Production guides & BOMs
│   ├── umg-si-furnace/          # UMG-Si arc furnace (Sand → Silicon)
│   ├── bio-leaching/            # Bio-leaching battery recycling
│   └── awg-unit/                # Atmospheric Water Generator
│
├── docs/                        # Documentation
│   ├── architecture.md          # System architecture overview
│   ├── getting-started.md       # How to contribute
│   ├── bom-guidelines.md        # Bill of Materials standards
│   ├── safety.md                # Electrical & mechanical safety
│   └── glossary.md              # Technical glossary (EN/AR)
│
├── CONTRIBUTING.md
├── LICENSE-HARDWARE              # CERN-OHL-P-2.0
├── LICENSE-SOFTWARE              # Apache-2.0
└── README.md                     # This file
```

---

## ⚡ Phase 1 — Energy Sovereignty

### SolarSync (Citizen Node)
| Spec | Value |
|------|-------|
| Solar Array | 5 kW (Tier-1 PV, >22% efficiency) |
| Storage | 10 kWh LFP (Lithium Iron Phosphate) |
| Water | AWG 20–30 L/day |
| Connectivity | LoRaWAN Gateway (868/915 MHz, 15km LOS) |
| Payment | Zero upfront — PAYGo model |

### OfficeSync (Commercial Hub)
| Spec | Value |
|------|-------|
| Solar Array | 20–50 kW |
| Storage | 40–100 kWh LFP |
| Compute | Micro-server (edge compute) |
| Compliance | On-chain ESG certificate |

### SFRES (Industrial Pillar)
| Spec | Value |
|------|-------|
| Solar Array | 250+ kW |
| Storage | 1+ MWh |
| Function | Battery swap hub + Factory host |

### LoRa Ghost Network
| Spec | Value |
|------|-------|
| Frequency | 868/915 MHz |
| Range | 15 km line-of-sight |
| Target Nodes | 205,000 |
| Encryption | End-to-end |
| Phase A | M2M telemetry only |
| Phase B | Full human mesh network (>100K nodes) |

### UMG-Si Manufacturing (Track B R&D)
Sand from Bara, North Kordofan (>98% purity) → Electric Arc Furnace → Directional Solidification → Plasma Purification → Solar-Grade Silicon (6N — 99.9999%).

### Bio-Leaching Recycling
Biological agents (A. ferrooxidans + A. niger) + organic acids from sugarcane/citrus waste → 90%+ battery material recovery rate. Zero chemical imports.

---

## 🚌 Phase 2 — Mobility Sovereignty

### Skateboard Chassis Platform
Universal EV platform shared across all vehicle types:
- **Axial-flux e-Axle**: High power density, hermetically sealed for desert conditions (50°C+), zero maintenance for 10+ years
- **Modular battery blocks**: Sub-3-minute hot-swap
- **Modular body mounting**: Supports trike, van, and bus configurations

### Vehicle Fleet
| Vehicle | Battery | Motor | Track | Use Case |
|---------|---------|-------|-------|----------|
| PulseTrike | 15 kWh | 5 kW | A | Urban rickshaw replacement |
| PulseVan | Modular | Modular | A→B | Logistics + harvest convoys |
| PulseBus | 4×50 kWh | Heavy | B | Mass transit (>5K fleet) |

### V2G (Vehicle-to-Grid)
10,000 parked buses = 2 GWh distributed storage. Smart contracts auto-discharge 15% during grid emergencies. Operators compensated via KWH-Tokens.

---

## 🌾 Phase 3 — Agricultural Sovereignty

### Autonomous Swarm (Track B)
| Robot | Function |
|-------|----------|
| Mother-Tractor 🚜 | Skateboard chassis, reads Soil DNA, precision Bio-Pod planting |
| Pulse-Rovers 🤖 | CNN vision, UV-C laser weeding, continuous root moisture sensing |
| Aero-Sentinels ✈️ | Autonomous daily sorties, NDVI mapping, early pest detection |

### Track A Prerequisites (Must complete first)
- Solar-powered irrigation pumps
- Post-harvest cold storage units (reduces 30%+ losses)
- SolarSync soil sensors → Building the Soil DNA database (3–5 years of mapping before robot deployment)

### Polyculture Matrix
Three crops grown simultaneously: sorghum 🌾, legumes 🌿, peanuts 🥜. Biological synergy (nitrogen fixation, shade canopy) doubles yield/hectare vs monoculture with zero chemical fertilizers.

### FaaS (Farming-as-a-Service)
1. Landowner draws boundaries on Mesh-ID
2. Ownership registered on-chain
3. Press "Deploy Swarm"
4. Protocol handles planting, harvesting, delivery

**Yield split:** 80% landowner · 15% protocol logistics · 5% UBI fund

### UBI Projections (Y1 → Y10)
| Year | Hectares (M) | Annual Pool ($M) | Per Family |
|------|-------------|-----------------|------------|
| Y1 | 0.5 | 27 | $3 |
| Y5 | 6 | 330 | $41 |
| Y10 | 20 | 1,100 | $135 |

---

## 🤝 Contributing

We welcome contributions from engineers, researchers, and makers worldwide. See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

Additional community docs:
- [Code of Conduct](./CODE_OF_CONDUCT.md)
- [Security Policy](./SECURITY.md)
- [Maintainers](./MAINTAINERS.md)
- [Roadmap](./ROADMAP.md)
- [Support](./SUPPORT.md)

### Current Project Status

This repository is in an **early foundation stage**. The structure and standards are defined, and we are actively onboarding contributors to build implementation modules across hardware, firmware, software, and manufacturing.

- ✅ Governance and contribution standards are available
- 🛠️ Most subsystem folders are currently scaffolded
- 🎯 Priority work is tracked through GitHub Issues and labels

**Priority areas:**
- KiCad schematics for SolarSync BMS
- Rust firmware for LoRa node
- Skateboard chassis FreeCAD models
- Soil DNA data pipeline architecture
- Arabic documentation translations

---

## 📜 Licensing

| Component | License |
|-----------|---------|
| Hardware designs | [CERN-OHL-P-2.0](./LICENSE-HARDWARE) |
| Firmware & Software | [Apache-2.0](./LICENSE-SOFTWARE) |
| Documentation | [CC-BY-SA-4.0](https://creativecommons.org/licenses/by-sa/4.0/) |

---

## 🌍 Mission

> *Build infrastructure that cannot be confiscated, destroyed by a single point of failure, or controlled by a central authority. Every watt generated, every kilometer traveled, and every grain harvested feeds a cycle of self-sufficiency.*

**بناء بنية تحتية لا يمكن مصادرتها، ولا تنهار بنقطة فشل واحدة، ولا تخضع لسلطة مركزية.**
