# Contributing to S.E.A.M Open

Thank you for your interest in contributing to the Sudan S.E.A.M Protocol! This project aims to build open-source infrastructure for Sudan's energy, mobility, and agriculture sovereignty.

## 🚀 How to Contribute

### 1. Find an Area
Browse the repository structure and pick an area that matches your expertise:

| Area | Skills Needed |
|------|---------------|
| `hardware/` | KiCad, FreeCAD, electrical engineering, mechanical design |
| `firmware/` | C, Rust, embedded systems, RTOS |
| `software/` | Python, TypeScript, blockchain, ML/AI |
| `manufacturing/` | Chemical engineering, materials science |
| `docs/` | Technical writing, Arabic translation |

### 2. Fork & Branch
```bash
git fork https://github.com/[org]/seam-open
git checkout -b feature/your-feature-name
```

### 3. Follow Standards

#### Hardware Designs
- Use **KiCad 8+** for PCB schematics and layouts
- Use **FreeCAD 0.21+** for mechanical CAD
- Every board must include a Bill of Materials (BOM) in CSV format
- Follow the BOM template in `docs/bom-guidelines.md`

#### Firmware
- Use **C17** or **Rust (stable)** for embedded code
- Target **STM32** (HAL) or **ESP32** (ESP-IDF) platforms
- All firmware must compile with no warnings (`-Wall -Werror`)
- Include a `platformio.ini` or `Cargo.toml` in each project root

#### Software
- Use **Python 3.11+** or **TypeScript (Node 20+)**
- Include unit tests (minimum 70% coverage for new modules)
- Use conventional commits: `feat:`, `fix:`, `docs:`, `refactor:`

### 4. Submit a Pull Request
- Write a clear description of what your PR does and why
- Reference related issues if applicable
- Ensure CI passes before requesting review

## 🌐 Language

- Code comments and variable names should be in **English**
- User-facing strings and documentation should provide **Arabic translations** where possible
- README files should be bilingual (English primary, Arabic secondary)

## 📋 Issue Labels

| Label | Meaning |
|-------|---------|
| `good-first-issue` | Beginner-friendly tasks |
| `hardware` | PCB, mechanical, or electrical work |
| `firmware` | Embedded systems work |
| `software` | Application or server-side work |
| `docs` | Documentation improvements |
| `research` | R&D investigation needed |
| `sudan-specific` | Requires local context or testing |

## ⚖️ Licensing

By contributing, you agree that your contributions will be licensed under:
- **CERN-OHL-P-2.0** for hardware designs
- **Apache-2.0** for firmware and software
- **CC-BY-SA-4.0** for documentation

## 🤝 Code of Conduct

Be respectful, inclusive, and constructive. We are building infrastructure for a nation — every contribution matters.
