# Getting Started

Welcome to the S.E.A.M Open project. This guide will help you set up your development environment and make your first contribution.

## Prerequisites

### Hardware Development
- **KiCad 8+** — PCB schematic and layout design
- **FreeCAD 0.21+** — Mechanical CAD modeling
- **LTspice** or **ngspice** — Circuit simulation (optional)

### Firmware Development
- **PlatformIO** or **STM32CubeIDE** — For C-based firmware
- **Rust toolchain** — `rustup` with `thumbv7em-none-eabihf` target
- **J-Link** or **ST-Link** — Debug probe

### Software Development
- **Python 3.11+** with `pip` or `uv`
- **Node.js 20+** with `npm`
- **Docker** — For local service orchestration

## Quick Start

```bash
# Clone the repository
git clone https://github.com/the-seam-protocol/seam-open.git
cd seam-open

# Pick a subsystem and navigate to it
cd firmware/solarsync-controller

# Follow the subsystem-specific README
```

## Project Board

Check the GitHub Issues and Projects board for open tasks tagged by area:
- `good-first-issue` — Start here
- `hardware`, `firmware`, `software` — Filter by skill
- `research` — Open investigations

## Communication

| Channel | Purpose |
|---------|---------|
| [Discord](https://discord.gg/HRYwPTB9) | Quick questions, community chat |
| [GitHub Discussions](https://github.com/the-seam-protocol/seam-open/discussions) | Design proposals and architecture threads |
| [GitHub Issues](https://github.com/the-seam-protocol/seam-open/issues) | Bug reports and task tracking |
| [Website](https://seam-protocol.sd) | Project overview and announcements |
