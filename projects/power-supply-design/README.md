# 🌊 Power Supply Design: 5V / 3.3V Dual Rail

> **Status:** 🟡 Simulation Verified | ⚪ PCB Not Fabricated

---

## 📐 Design Specifications

* **Input:** 9V – 12V DC
* **Output A:** 5V @ 1.5A (Buck Converter)
* **Output B:** 3.3V @ 500mA (LDO for low-noise rail)
* **Target Ripple:** < 20mV peak-to-peak

---

## ⚙️ Circuit Architecture

This design uses a **two-stage regulation approach**:

1. **Buck Converter (Step-Down Switching Regulator)**

   * Converts 9–12V input to stable 5V output
   * Designed for improved efficiency under load

2. **LDO Regulator (Low-Dropout Linear Regulator)**

   * Steps 5V down to 3.3V
   * Provides low-noise output for sensitive components

---

## 🛠️ Key Components

* **Buck Converter:** LM2596 (Step-down regulator)
* **LDO Regulator:** AMS1117-3.3
* **Inductor:** 33µH shielded high-current inductor
* **Capacitors:** Input/output filtering for ripple reduction

---

## 🔬 Simulation Results (LTspice / Ngspice)

I simulated the circuit using **Transient Analysis** to evaluate startup behavior and load response.

* **Startup Time:** < 5ms to steady state

### Load Step Response:

* 0.5A → 1.5A transition
* Voltage sag: ~150mV
* Recovery time: ~200µs

---

## 📈 Results Summary

* Stable 5V output under dynamic load conditions
* Fast transient recovery (~200µs)
* Minimal voltage sag during load spikes (~150mV)
* Clean 3.3V rail using LDO regulation

---

## 📸 Design & Simulation Preview

### 🔌 Schematic

![Schematic](images/schematic.png)

### 📊 Transient Response

![Transient](images/transient.png)

---

## 📂 File Directory

* `/schematics` → (Planned for KiCad schematic files)
* `/pcb` → (Planned for PCB layout and Gerber files)
* `/simulation` → `.asc` SPICE simulation files

---

## 🧪 Testing Approach

* Input variation across 9V–12V
* Load testing from 0.5A to 1.5A
* Startup transient analysis
* Voltage stability verification

---

## ⚠️ Design Considerations

* Switching regulator introduces ripple (mitigated via filtering)
* LDO used to ensure clean 3.3V output
* Thermal performance depends on load conditions

---

## 🚀 Future Improvements

* PCB layout and routing using KiCad
* Hardware prototype validation
* Thermal analysis under full load
* Efficiency optimization

---

## 🔗 Navigation

[⬅ Back to Main Portfolio](../../README.md)
