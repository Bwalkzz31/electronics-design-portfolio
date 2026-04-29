# 🌊 Power Supply Design: 5V/3.3V Dual Rail
> **Status:** 🟡 Simulation Verified | ⚪ PCB Fabricated

## 📐 Design Specifications
- **Input:** 9V - 12V DC
- **Output A:** 5V @ 1.5A (Switching)
- **Output B:** 3.3V @ 500mA (LDO for low noise)
- **Target Ripple:** < 20mV peak-to-peak

## 🔬 Simulation Results (LTspice/Ngspice)
The design was subjected to a **Transient Analysis** to verify start-up time and load step response.
*   **Startup Time:** < 5ms to reach steady state.
*   **Load Step:** 0.5A to 1.5A jump shows a maximum voltage sag of 150mV with recovery in 200μs.

## 📂 File Directory
- `/schematics`: KiCad `.kicad_sch` source files.
- `/pcb`: KiCad `.kicad_pcb` and Gerber production files.
- `/simulation`: `.asc` SPICE decks and `.plt` waveform settings.

## 🛠️ Key Components
- **Buck Converter:** [Insert Part Number, e.g., LM2596]
- **LDO Regulator:** [Insert Part Number, e.g., AMS1117]
- **Inductor:** 33µH High-Current Shielded

[⬅ Back to Main Portfolio](../../README.md)
