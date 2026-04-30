# 🔬 SPICE Simulation & Convergence Guide
> **Goal:** High-accuracy transient and AC analysis without simulation crashes.

In electronics design, "chaos" often manifests as convergence errors—where the math behind the circuit becomes too complex for the simulator to solve. This guide outlines the protocol used in this portfolio to ensure SPICE simulations are stable and physically accurate.

## 🚀 Common Convergence Fixes
If a simulation fails to start, stalls at 0%, or produces "Timestep too small" errors, try these adjustments:

1.  **GMIN Stepping:** Increase `GMIN` (the minimum conductance allowed) slightly to help the solver find a DC operating point.
    *   *Command:* `.options gmin=1e-10`
2.  **Integration Method:** Switch from `TRAP` (Trapezoidal) to `GEAR`. Trapezoidal is faster but can cause "ringing" artifacts; Gear is more stable for switching power supply (SMPS) simulations.
    *   *Command:* `.options method=gear`
3.  **Slew Rate Control:** Ensure your voltage sources have realistic rise/fall times (e.g., 10ns) instead of 0ns. Infinite slopes cause mathematical singularities that crash the solver.
4.  **Abstol/Reltol:** Slightly relaxing the tolerance can help the simulation finish without sacrificing significant accuracy.
    *   *Command:* `.options reltol=0.01 abstol=1n`

## 📈 Standard Analysis Protocol
To "tame the storm," every analog circuit in this repository undergoes:
*   **DC Operating Point (`.op`):** Verifying bias voltages and quiescent current.
*   **Transient Analysis (`.tran`):** Checking time-domain behavior, ripple, and "water-crash" stress events.
*   **AC Analysis (`.ac`):** Evaluating frequency response, phase margin, and filter roll-off.

---
[⬅ Back to Main Portfolio](../../README.md)
