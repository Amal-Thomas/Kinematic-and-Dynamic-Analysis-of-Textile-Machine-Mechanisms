# Kinematic-and-Dynamic-Analysis-of-Textile-Machine-Mechanisms
## ME 754 - Textile Machines Design & Automation

**Author:** Amal Thomas

---

## Overview

This repository contains two project reports for ME754, each analysing a real-world textile machine mechanism in ADAMS software, including kinematic and dynamic simulations, manual calculations, and comparison against an alternate 4-bar linkage.

---

## Repository Contents

### 1. `Sulzer-torsion_picking_mechanism.pdf` — Sulzer-Torsion Picking Mechanism
An analysis of the shuttle picking mechanism used in Sulzer projectile looms, covering:
- **Mechanism description**: cam-driven system with a torsion spring, operating at 75 rpm (150 picks/min with two alternating mechanisms); output point P on L-shaped link 1 (ternary linkage)
- **Kinematic simulation**: displacement (X and Y vs. time), path trace, velocity, and acceleration profiles; point P remains idle for most of the cycle, with a sharp high-speed picking action (~800 mm/s peak velocity)
- **Dynamic simulation**: total mechanism mass 19.982 kg; average torque 3.143 Nm; average power 24.688 W; peak power 541.29 W
- **Alternate linkage**: 4-bar crank-rocker mechanism at the same 75 rpm; total mass 8.746 kg; average torque 0.24 Nm; average power 1.886 W; peak power 5.433 W
- **Manual kinematic analysis** of the alternate linkage using geometric constraint equations and numerical differentiation
- **Comparison and index of merit**: original mechanism is functionally superior (high-momentum impulsive pick, idle dwell period, torsion spring energy storage) despite higher vibrations and torque demand; alternate mechanism is smoother but incapable of the required impulsive picking action

---

### 2. `Ashford_spinning_wheel_treadle_mechanism.pdf` — Ashford Spinning Wheel Treadle Mechanism
An analysis of the treadle mechanism of the Ashford traditional spinning wheel, covering:
- **Mechanism description**: foot-operated crankshaft and connecting rod system driving a 360 mm diameter flywheel at 500 rpm; out-of-plane linkages connected via a string/spring; 400 N foot force applied in simulation; output is foot pedal center of mass (point P)
- **Kinematic simulation**: mechanism rotated 90° to plot motion in XY plane; displacement, trace, velocity (~2000 mm/s peak), and acceleration profiles; vibrations attributed to the out-of-plane string connection between the rocker and connecting rod
- **Dynamic simulation**: total mechanism mass 7.348 kg; average torque 12.673 Nm; average power 663.545 W; peak power 2074.35 W
- **Alternate linkage**: planar 4-bar crank-rocker mechanism (bevel gears omitted for simplicity); total mass 3.712 kg; average torque 14.991 Nm; average power 784.93 W; peak power 1579.07 W
- **Manual kinematic analysis** of the alternate linkage with full geometric derivation of φ as a function of θ using the BC distance constraint
- **Comparison and index of merit**: original mechanism is preferable from a user and repairability standpoint (foot-operated, lower average power, easy to maintain); alternate mechanism produces smoother operation but requires bevel gears, consumes more average power, and is less practical in a home/traditional setting

---
