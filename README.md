# Aqua Pulse — Industrial Water Purification & Sensor Digital Twin 💧⚙️

> **Smart India Hackathon (SIH 2026)**  
> **Problem Statement ID:** SIH26040 — Smart Hardware  
> **Standards:** WHO / BIS IS 10500 Compliant Architecture  
> **Tech Stack:** WebGL, Three.js, HTML5 Canvas, SCADA Telemetry Engine

---

## 🌊 Overview

**Aqua Pulse 3D Digital Twin** is an interactive, physically-accurate 3D simulation and SCADA telemetry skid of an industrial multi-stage water purification station. It provides real-time fluid dynamics visualization, sensor telemetry streaming at 10Hz, automated divert gates, and deep component-level technical specifications.

---

## ✨ Features

- **Physically Routed 3D Piping Network:** Dual continuous blue (potable permeate) and orange (brine/reject) flow paths.
- **Particle Fluid Dynamics:** 180+ animated fluid particles dynamically changing color across treatment stages (turbid yellow-brown -> sediment-cleared -> UV-excited violet -> ultra-pure electric turquoise).
- **13 Selectable Hardware Modules:**
  1. Heavy-Duty Structural 6061-T6 Aluminum Skid Chassis
  2. Raw Water Source Vessel & Sight Level Tube
  3. High-Pressure Diaphragm Booster Pump (60–75 PSI)
  4. **In-Line DS18B20 Submersible Digital Temperature Sensor Probe**
  5. Multi-Sensor Analytical Flow Cell (Turbidity, pH, TDS/EC, Hall-effect flow turbine)
  6. Stage 1: 5μm Spun Polypropylene Sediment Filter
  7. Stage 2: Extruded Activated Carbon Block (CTO)
  8. Stage 3: Thin-Film Composite (TFC) RO Membrane Vessel
  9. Stage 4: 254nm UV-C Germicidal Disinfection Reactor
  10. Fail-Safe 3-Way Solenoid Diverter Gate
  11. Clean Potable Effluent Reservoir & Dispenser
  12. ESP32-S3 IoT Brain with Dynamic Mini OLED Display
  13. 100W Solar PV & 24V LiFePO4 Battery Off-Grid Power Skid
- **Live 10Hz SCADA Telemetry Stream:** Real-time turbidity (NTU), total dissolved solids (ppm), pH, temperature (°C), flow rate (L/min), pressure (PSI), and UV-C intensity (%).
- **Interactive Simulation Controls:**
  - ⚡ Booster Pump On/Off toggle
  - ⚠️ Contamination Spike Injection & Automated Solenoid Divert Interlock
  - 👁️ Canister X-Ray / Transparent Shell Mode
  - 💧 Flow Particle Dynamics Toggle
  - 📦 Exploded CAD Assembly View
  - 🔄 Auto-Rotate & Orbit Controls
- **CAD Camera Presets:** Overview (Iso), Temp Probe, Sensors Flow Cell, Filtration Skid, ESP32 Brain, Top Plan.

---

## 🚀 Quick Start

No build tools required! Simply open `index.html` or serve via any static HTTP server:

```bash
# Using Python
python -m http.server 8080

# Using Node
npx serve .
```

Open [http://localhost:8080](http://localhost:8080) in any modern web browser with WebGL support.
