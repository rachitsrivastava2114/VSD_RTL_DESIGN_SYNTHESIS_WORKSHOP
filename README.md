# VSDIAT RTL Design & Synthesis Workshop 🚀
**Created by Rachit Srivastava**

[![Toolchain](https://img.shields.io/badge/Toolchain-iverilog%20%7C%20GTKWave%20%7C%20Yosys-blueviolet)](#)
[![PDK](https://img.shields.io/badge/PDK-Sky130-orange)](#)

This repository documents the complete **RTL-to-GDS front-end flow** using open-source tools and the Sky130 PDK. Over the course of 5 days, I explored behavioural Verilog simulation, logic synthesis, hierarchical design strategies, and gate-level verification.

---

## 🛠️ Toolchain & Environment
- **Simulator:** [Icarus Verilog](http://iverilog.icarus.com/) (Functional Verification)
- **Waveform Viewer:** [GTKWave](http://gtkwave.sourceforge.net/) (Signal Analysis)
- **Synthesis Tool:** [Yosys](https://yosyshq.net/yosys/) (RTL to Netlist)
- **Standard Cells:** [Sky130 PDK](https://github.com/google/skywater-pdk) (Foundry Data)

---

## 🗺️ Curriculum Roadmap

### [☀️ Day 1: Simulation Basics with iVerilog](#day-1-simulation-basics-with-iverilog)
### [☀️ Day 2: Logic Synthesis with Yosys](#day-2-logic-synthesis-with-yosys)
### [☀️ Day 3: Libraries and Hierarchy](#day-3-libraries-and-hierarchy)
### [☀️ Day 4: Sequential Logic & Optimisations](#day-4-sequential-logic--optimisations)
### [☀️ Day 5: GLS & Final Sign-off](#day-5-gls--final-sign-off)

---

## 🔬 Detailed Lab Walkthrough

### Day 1: Simulation Basics with iVerilog
**Theory:** Simulation verifies functional correctness. We use a Testbench to drive inputs to the DUT and capture signals in a `.vcd` file.

| Description | Image |
| :--- | :--- |
| **Terminal Setup** | ![Setup](./module_1/sim/labs_using_iverilog_gtk-lec1/part12.png) |
| **VCD Generation** | ![VCD](./module_1/sim/labs_using_iverilog_gtk-lec1/part14.png) |
| **GTKWave Launch** | ![Launch](./module_1/sim/labs_using_iverilog_gtk-lec1/part15.png) |
| **2:1 MUX Waveform** | ![Waveform](./module_1/sim/labs_using_iverilog_gtk-lec1/part16.png) |
| **Zoomed Analysis** | ![Zoom](./module_1/sim/lec2/part21.png) |
| **Signal Toggles** | ![Toggles](./module_1/sim/lec2/part22.png) |
| **Bug Detection** | ![Bug](./module_1/sim/lec3/part31.png) |
| **Final Verification** | ![Final](./module_1/sim/lec3/part32.png) |

---

### Day 2: Logic Synthesis with Yosys
**Theory:** Synthesis converts RTL to gates. Yosys maps logic to Sky130 cells using the `abc` tool.

| Step | Output / Schematic |
| :--- | :--- |
| **Reading Libs** | ![Read](./module_1/synth/part41.png) |
| **Synthesis Run** | ![Synth](./module_1/synth/part42.png) |
| **Gate Schematic** | ![Schem](./module_1/synth/part51.png) |
| **Netlist Detail** | ![Detail](./module_1/synth/part52.png) |
| **Area Stats** | ![Stats](./module_1/synth/part53.png) |
| **Verilog Netlist** | ![Netlist](./module_1/synth/part54.png) |
| **Optimisation** | ![Opt](./module_1/synth/part61.png) |
| **Netlist Check** | ![Check](./module_1/synth/part62.png) |

---

### Day 3: Libraries and Hierarchy
**Theory:** Exploring PVT corners and Hierarchical vs Flat synthesis.

| Concept | Visualization |
| :--- | :--- |
| **Sky130 Lib** | ![Lib](./module_1/pdk/part71.png) |
| **Cell Models** | ![Models](./module_1/pdk/part72.png) |
| **Hierarchical Map** | ![Hier](./module_1/pdk/part74.png) |
| **Flat Synthesis** | ![Flat](./module_1/pdk/part75.png) |
| **Mapping Stats** | ![Stats](./module_1/pdk/part76.png) |
| **Hierarchy Flow** | ![Flow](./module_2/hierarchy/4.png) |

---

### Day 4: Sequential Logic & Optimisations
**Theory:** D-Flip Flops, resets, and glitch analysis.

| Lab | Result |
| :--- | :--- |
| **DFF Async Reset** | ![DFF1](./module_2/flops/1.png) |
| **DFF Sync Reset** | ![DFF2](./module_2/flops/3.png) |
| **DFF Clock Enable** | ![DFF3](./module_2/flops/5.png) |
| **Glitch Analysis** | ![Glitch](./module_2/flops/7.png) |
| **Logic Pruning** | ![Pruning](./module_2/flops/9.png) |

---

### Day 5: GLS & Final Sign-off
**Theory:** Gate Level Simulation for post-synthesis verification.

| Milestone | Waveform / Log |
| :--- | :--- |
| **GLS Waveform** | ![GLS1](./module_1/pdk/part91.png) |
| **Functional Match** | ![GLS2](./module_1/pdk/part92.png) |

---

## 🏁 Conclusion
Through this workshop, I successfully implemented a complete front-end ASIC flow. The project demonstrates the power of open-source EDA tools in designing silicon-ready logic.

## 🖼️ Full Project Gallery

To ensure complete documentation, here is the full set of lab artifacts captured during the workshop.

| | | |
| :---: | :---: | :---: |
| ![1](./results/1.png) | ![2](./results/2.png) | ![3](./results/3.png) |
| ![4](./results/4.png) | ![5](./results/5.png) | ![6](./results/6.png) |
| ![7](./results/7.png) | ![8](./results/8.png) | ![9](./results/9.png) |
| ![10](./results/10.png) | ![11](./results/11.png) | ![12](./results/12.png) |
| ![13](./results/13.png) | ![part_11](./results/part_11.png) | ![part13](./results/part13.png) |
| ![part14](./results/part14.png) | ![part15](./results/part15.png) | ![part23](./results/part23.png) |
| ![part72](./results/part72.png) | ![part73](./results/part73.png) | ![part75](./results/part75.png) |

---
**Created by Rachit Srivastava**  
*VSDIAT - Digital Design Program*
