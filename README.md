# ⚡ Electronics Design & Simulation Portfolio

Designed and simulated a regulated DC power supply using circuit design principles and SPICE-based analysis. This project focuses on voltage regulation, ripple suppression, and performance under varying load and input conditions.

---

## 📌 Project Overview

Designed and simulated a **5V regulated DC power supply** capable of maintaining stable output across varying input voltages and dynamic load conditions.

The design was analyzed using **LTspice**, with emphasis on:

* Voltage regulation accuracy
* Ripple suppression
* Transient response under load variation

The system was tested across multiple operating scenarios to evaluate stability, efficiency, and response to dynamic load changes.

---

## 📊 Performance Results

Simulation results confirm stable operation across tested conditions:

* **Output Voltage:** 5V ±1%
* **Output Ripple:** < 50mV peak-to-peak
* **Load Stability:** Maintained across 0.1A to 1A
* **Line Regulation:** Stable across 7V–12V input range

---

## 📈 Results Summary

* Stable output under dynamic load conditions
* Fast transient response during load changes
* Minimal voltage deviation across input range
* Reliable performance in both steady-state and transient scenarios

---

## 📸 Design & Simulation Preview

![Power Supply Schematic and Transient Response](projects/power-supply-design/images/schematic.png)


---

## 🧪 Simulation Methodology

* **Tool Used:** LTspice
* **Analysis Types:**

  * Transient Analysis (startup behavior and voltage stability)
  * AC Analysis (ripple and noise evaluation)

### Input Conditions:

* Input Voltage Range: 7V–12V
* Load Range: 0.1A – 1A

### Measurement Points:

* Output Voltage (Vout)
* Ripple amplitude
* Stability under dynamic load conditions

---

## ⚙️ Design Approach

The system was designed using a **linear voltage regulation topology** to prioritize low noise and stable output.

Key considerations included:

* Maintaining consistent voltage across variable load conditions
* Minimizing ripple through capacitor selection
* Ensuring stable transient response during load switching

Simulations were used to validate performance and identify potential instability under edge conditions.

---

## 🧠 Design Decisions

* **Regulator Selection:**
  Linear regulator chosen for low-noise output and simplicity

* **Capacitor Sizing:**
  Balanced ripple reduction with transient response performance

* **Input Range Handling:**
  Designed to operate reliably across a 7V–12V range

* **Stability Considerations:**
  Verified no oscillation under varying load conditions

---

## 🧪 Test Scenarios

* Startup response under nominal input voltage
* Load variation from 0.1A to 1A
* Input voltage fluctuation (7V–12V range)
* Ripple measurement under steady-state conditions

---

## ⚠️ Limitations & Considerations

* Lower efficiency compared to switching regulators
* Increased heat dissipation at higher load currents
* Design prioritizes stability and low noise over efficiency

Future iterations could incorporate switching regulation to improve efficiency while maintaining acceptable ripple levels.

---

## 🚀 How to Reproduce

1. Open LTspice
2. Navigate to `/simulations/power_supply.asc`
3. Run transient simulation
4. Observe output at node `Vout`
5. Modify load resistance to test different load conditions

---

## 🛠️ Tools & Technologies

* LTspice (Circuit Simulation)
* Circuit Design & Analysis
* Electrical Debugging Techniques

---

## 📁 Repository Structure

```
electronics-design-simulation/
│
├── projects/
│   └── power-supply-design/
│       ├── images/
│       │   └── schematic.png
│       ├── simulation/
│       │   └── power_supply.asc
│       └── README.md
│
└── README.md
```

---

## 📌 Future Improvements

* PCB design and layout using KiCad
* Hardware prototype implementation
* Integration with microcontroller-based monitoring
* Exploration of switching regulator design for improved efficiency

---

## 👤 Author

**Britany Walker**
IT Management Student | Aspiring IT & Systems Professional

* GitHub: https://github.com/Bwalkzz31
* Portfolio: https://bwalkzz31.github.io

---
