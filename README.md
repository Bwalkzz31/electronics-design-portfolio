<p align="center">
  <img src="assets/banner.svg" alt="Electronics Portfolio Banner" width="100%">
</p>

# ⚡ Electronics Design & Simulation Portfolio

Focused on entry-level and contract opportunities in **Electronics Design & Simulation (EDA)**.

Hands-on portfolio demonstrating practical experience in **circuit design, PCB development, and simulation-driven validation** using industry-standard tools.

This work reflects a strong understanding of **circuit behavior, performance validation, and engineering workflows** aligned with real-world electronics development.

---

## 🚀 Project Snapshot

**Project:** Dual Rail Power Supply (5V / 3.3V)  
**Tools:** KiCad, NGSpice, LTSpice  
**Focus:** Circuit Design • Simulation • Power Integrity • Validation  

### Key Results

- Maintained 5V output within **4.95V – 5.05V**
- Maintained 3.3V output within **3.25V – 3.35V**
- Achieved low ripple between **20mV – 50mV** under load
- Transient recovery time **< 2ms** during step-load changes
- Stable operation across **0mA – 500mA** load range

---

## 📸 Design & Simulation Preview

> Representative outputs from schematic design and SPICE-based validation.  
> Images will be added as the project progresses.

<!--
<p align="center">
  <img src="projects/power-supply-design/images/schematic.png" alt="Power Supply Schematic" width="48%">
  <img src="projects/power-supply-design/images/simulation.png" alt="SPICE Simulation Output" width="48%">
</p>
-->

---

## 📌 Overview

This portfolio highlights applied experience in:

- Power supply design and voltage regulation
- Analog signal processing and conditioning
- Circuit simulation and performance validation
- PCB layout and system-level design

All work follows a **simulation-first engineering approach**, validating circuit behavior across multiple operating conditions before implementation.

---

## 🛠 Tools & Technologies

- **PCB Design:** KiCad
- **Simulation:** NGSpice, LTSpice
- **Analysis:** DC, AC, Transient simulations
- **Outputs:** Schematics, PCB layouts, simulation waveforms, BOMs

---

## 🚀 Featured Project

### ⚡ Dual Rail Power Supply (5V / 3.3V)

#### 📖 Description

Designed and simulated a dual-output regulated power supply delivering stable **5V and 3.3V rails**.

The system is designed to maintain voltage stability under varying load conditions while minimizing ripple through filtering, decoupling, and regulation techniques.

---

#### ⚙️ Key Features

- Dual regulated voltage outputs: **5V and 3.3V**
- Linear voltage regulation architecture
- Input filtering and decoupling for noise reduction
- Stable performance under dynamic load conditions

---

#### 🔍 Design Decisions

- Selected linear regulation for simplicity, low noise, and predictable output behavior
- Used filtering and decoupling capacitors to reduce ripple and improve voltage stability
- Evaluated performance under multiple load conditions to confirm reliability
- Prioritized stable transient response during step-load changes

---

#### 🧪 Simulation & Validation

SPICE-based simulation was used to evaluate:

- Load regulation across operating range
- Output ripple under varying load conditions
- Transient response during step-load changes
- Voltage stability across no-load, medium-load, and full-load scenarios

---

#### 🧪 Test Conditions

Simulated across realistic load scenarios:

- No load: **0mA**
- Medium load: **250mA**
- Full load: **500mA**

Step-load transitions were applied to analyze system stability and recovery behavior.

---

#### 📊 Performance Results

- **5V Rail:** 4.95V – 5.05V
- **3.3V Rail:** 3.25V – 3.35V
- **Ripple Voltage:** 20mV – 50mV
- **Transient Response:** < 2ms recovery time
- **Load Stability:** Maintained across full load range

---

#### ⚠️ Engineering Challenge

Power supply designs must maintain stable output voltage even when load conditions change quickly.

Step-load behavior was reviewed to evaluate whether the output rails could recover quickly without excessive ripple or voltage deviation.

---

#### ✅ Solution

Filtering, decoupling, and regulation were used to improve stability and reduce ripple. Simulation results confirmed that the design maintained stable voltage output across tested load conditions.

---

#### 📦 Project Artifacts

- Schematic design files
- PCB layout structure
- SPICE simulation notes
- Simulation waveforms
- Bill of Materials planning
- Convergence and simulation troubleshooting guide

---

#### 💡 Engineering Insight

This project demonstrates a structured approach to designing and validating stable power delivery systems.

Key engineering considerations include:

- Minimizing ripple through filtering and decoupling
- Maintaining voltage regulation across load variation
- Ensuring fast and stable transient response
- Validating circuit behavior before physical implementation

A simulation-driven workflow was used to reduce design risk and verify performance prior to implementation.

---

## 🔬 Additional Project Planned

### 📡 ADC Interface Board

#### 📖 Description

Designing an analog-to-digital interface for accurate signal acquisition and digital conversion.

---

#### 🎯 Objectives

- Signal conditioning and filtering
- Noise reduction and stability
- Accurate sampling and data integrity
- Reliable analog-to-digital signal conversion

---

#### 🧪 Current Status

- Schematic design planned
- Component selection in progress
- Simulation phase planned

---

## 🧠 Design Approach

- **Schematic-First Design:** Define system architecture before implementation
- **Simulation-Driven Validation:** Verify performance prior to PCB layout
- **Performance-Focused Engineering:** Prioritize stability, efficiency, and reliability
- **Iterative Development:** Refine designs through testing and analysis
- **Documentation-Driven Workflow:** Maintain clear notes, outputs, and engineering decisions

---

## 📈 Progress

- [x] Portfolio structure created
- [x] Power supply project documented
- [x] Simulation analysis documented
- [x] Convergence and simulation guide added
- [ ] Real schematic screenshot added
- [ ] Real simulation waveform screenshot added
- [ ] PCB layout finalization
- [ ] ADC interface design completion

---

## 📂 Repository Structure

```text
electronics-design-simulation/
│
├── assets/
│   ├── banner.svg
│   ├── analog-chaos.jpg
│   └── digital-sampling.jpg
│
├── projects/
│   └── power-supply-design/
│       ├── schematics/
│       ├── pcb/
│       ├── simulations/
│       └── images/
│
├── convergence-tips.md
├── README.md
└── LICENSE
