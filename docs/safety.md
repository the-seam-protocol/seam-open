# Safety Guidelines

## ⚡ Electrical Safety

### High Voltage Systems (SolarSync, SFRES)
- All systems above 48V DC must include **ground fault detection**
- Arc-fault circuit interrupters (AFCI) required on all PV string combiners
- Lockout/tagout procedures documented for every maintenance operation
- Minimum **IP65** rating for all junction boxes

### Battery Safety (LFP Cells)
- BMS must enforce per-cell voltage limits: **2.5V min — 3.65V max**
- Temperature cutoff at **60°C** (charge) and **65°C** (discharge)
- Mechanical enclosures must pass **UN38.3** transport safety testing
- Fire-resistant separators between cell modules

### Battery Swap Stations
- Interlock prevents swap while vehicle is in motion
- Connector rated for **200A continuous** with arc suppression
- Emergency stop (E-STOP) button accessible from all sides

## 🔧 Mechanical Safety

### Desert Environment
- All outdoor enclosures: **IP65** minimum, **IP67** for ground-level
- UV-stabilized plastics or powder-coated aluminum
- Sand ingress protection on all air intakes (filtered vents)
- Operating temperature: **-10°C to +70°C**

### Vehicle Systems
- Roll cage structure on all PulseBus frames
- Battery pack crash protection (side impact rated)
- Thermal runaway venting directed away from passenger cabin

## 📡 RF Safety

### LoRa Network
- Transmit power limited to regional regulations (868 MHz EU: 25 mW ERP / 915 MHz: 1W)
- Antenna placement >30cm from human body during transmission
- SAR compliance for any wearable or body-mounted nodes

## ⚠️ General Rules

1. **Never** bypass a BMS or safety interlock
2. **Always** de-energize before servicing
3. **Document** all safety-critical design decisions in the relevant subsystem README
4. **Test** thermal runaway scenarios in simulation before physical prototyping
