<div align="center">
  <img src="assets/banner.svg" alt="Water Crashing on Circuit — Electronics Design Portfolio" width="100%">
  <h1>⚡ ELECTRONICS DESIGN PORTFOLIO</h1>
  <p><strong>Where water meets wire — a master-level collection of EDA projects, simulations, and hardware designs</strong></p>
  <p>
    <img src="https://img.shields.io/badge/Domain-PCB%20Design-cyan?style=flat-square">
    <img src="https://img.shields.io/badge/Domain-SPICE%20Simulation-magenta?style=flat-square">
    <img src="https://img.shields.io/badge/Domain-Digital%20Logic-gold?style=flat-square">
    <img src="https://img.shields.io/badge/License-MIT-blue?style=flat-square">
  </p>
</div>

---

## 🌊 The Concept
*Water crashing on a circuit* — the moment fluid chaos meets rigid structure, where raw energy discharges across traces designed for control. This portfolio captures that spirit: the collision of creativity with precision engineering, of organic problem-solving with the disciplined art of electronics design.

Every schematic is a controlled path through chaos. Every simulation is a prediction of how energy will flow. Every PCB layout is an attempt to tame the storm.

---

## 🛠️ Tools & Stack


| Domain | Primary Tools | Output Formats |
| :--- | :--- | :--- |
| **Schematic & PCB** | KiCad 8, KiCad 7 | `.kicad_sch`, `.kicad_pcb` |
| **SPICE Simulation** | LTspice XVII, Ngspice, Qucs-S | `.asc`, `.cir`, `.sp` |
| **Analysis Types** | AC, DC, Transient, S-Parameters | `.raw`, `.log`, `.plt` |
| **Fabrication** | Gerber RS-274X, Excellon, IBOM | `.gbr`, `.drl`, `.pos` |
| **Documentation** | Markdown, LaTeX, KiCad PDF | `.md`, `.tex`, `.pdf` |

---

## 🔧 Featured Projects

### 🌊 [Power Supply Design (The Storm)](projects/power-supply-design/)
<img src="assets/analog-chaos.jpg" width="100%" alt="Analog Chaos - Power Supply">

> **Focus: Stability Under Stress.** 
> A robust 5V/3.3V dual-rail regulator designed to maintain rock-solid stability even when electrical "chaos" hits the traces.
*   **Engineering Challenge:** Balancing high-efficiency thermal dissipation with ultra-fast transient response.
*   **Status:** 🟡 In Progress — *Finalizing Thermal Derating Curves.*

---

### 💧 [ADC Interface Board (The Precision)](projects/adc-interface-board/)
<img src="assets/digital-sampling.jpg" width="100%" alt="Digital Precision - ADC Interface">

> **Focus: Capturing the Drop.** 
> A 16-bit SAR ADC breakout that captures fluid analog signals and quantizes them into precise digital data with zero "splash."
*   **Engineering Challenge:** Designing an Anti-Alias Filter (AAF) to prevent signal ghosting and ensuring SPI data integrity.
*   **Status:** 🔵 Planned — *Component sourcing in progress.*

---

## 📂 Repository Structure

```text
electronics-design-portfolio/
├── assets/                    # Project visual assets (banners, icons)
├── projects/
│   ├── power-supply-design/   # Schematics, PCB, and SPICE decks
│   ├── adc-interface-board/   # 16-bit SAR ADC files
│   └── mixed-signal-filter/   # Active Butterworth filter design
├── docs/
│   ├── simulation-guides/     # SPICE tips and convergence helpers
│   └── pcb-guidelines/        # DRC rules and stackup references
├── README.md
└── LICENSE
```

---

## 📐 Design Philosophy

**Schematic First, Always.** No auto-routed shortcuts. Every net is intentional, every component selected with purpose.

**Simulate Before You Fabricate.** SPICE is the rehearsal before the performance. Transient analysis and AC sweeps are mandatory before layout begins.

**Chaos is the Test.** A design must survive the storm. Power ripple, EMI, and thermal drift are the "water" our circuits must withstand.

---

## 🖥️ Simulation Workflow

```text
  ┌─────────────┐     ┌──────────────┐     ┌─────────────┐
  │  Schematic   │────▶│  SPICE Deck  │────▶│  Simulate   │
  │  Capture     │     │  Generation  │     │  (Ngspice)  │
  └─────────────┘     └──────────────┘     └──────┬──────┘
                                                   │
                                                   ▼
  ┌─────────────┐     ┌──────────────┐     ┌─────────────┐
  │  PCB Layout  │◀────│  Validate &  │◀────│  Analyze    │
  │  (KiCad)    │     │  Iterate     │     │  Results    │
  └─────────────┘     └──────────────┘     └─────────────┘
```

1.  **Capture** — Draw the schematic in KiCad with proper symbol libraries and annotations.
2.  **Generate** — Export the SPICE netlist with model references and sub-circuit definitions.
3.  **Simulate** — Run DC, AC, and transient analyses in Ngspice or LTspice.
4.  **Analyze** — Review waveforms, check margins, verify stability and bandwidth.
5.  **Validate** — Confirm results meet specifications; iterate if needed.
6.  **Layout** — Proceed to PCB layout only after simulation validation passes.

---

## 📋 Progress Tracker

- [x] Repository structure and branding established
- [x] Hero banner and visual identity created
- [x] Documentation — [Simulation Guide](convergence-tips.md) completed
- [ ] Power Supply Design — Schematic capture
- [ ] Power Supply Design — SPICE simulation suite
- [ ] ADC Interface Board — Schematic and component selection
- [ ] Mixed-Signal Filter — Topology selection and simulation

---

## 🤝 Contributing
This is a personal portfolio, but suggestions are welcome. Open an issue or submit a pull request if you spot a way to improve a design.

---

## 📄 License
This project is licensed under the MIT License.
