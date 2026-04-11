# Bill of Materials (BOM) Guidelines

## Format

All BOMs must be provided as CSV files with the following columns:

```csv
Reference,Value,Footprint,Quantity,Manufacturer,MPN,Supplier,SupplierPN,UnitCost_USD,Notes
```

## Rules

1. **Local sourcing priority** — Prefer components available in East Africa or Middle East supply chains
2. **Heat tolerance** — All components must be rated for **-10°C to +70°C** operating range (Sudan desert conditions)
3. **IP rating** — Outdoor-exposed components must be **IP65** minimum
4. **Lead-free** — All solder and components must be RoHS compliant
5. **Standardization** — Reuse the same component across subsystems where possible (e.g., same LFP cell chemistry across SolarSync, PulseTrike, PulseBus)

## Cost Targets

| Subsystem | Target BOM Cost |
|-----------|----------------|
| SolarSync (5kW) | < $2,500 |
| PulseTrike battery (15kWh) | < $4,000 |
| LoRa Gateway | < $50 |
| LoRa Node | < $15 |
| Soil Sensor Module | < $25 |
