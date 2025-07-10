# ⚙️ Power-Efficient VLSI Architecture of Finite State Vending Machine

## 📌 Project Overview

This project presents a **Finite State Machine (FSM)** based **Vending Machine Controller** designed using **power-efficient VLSI techniques**. The design is implemented at the RTL level using **Verilog/VHDL**, focusing on **area, timing, and power optimization** during synthesis.

The vending machine dispenses items based on coin input and product selection, with built-in change return and idle state control. This architecture is optimized for **low power consumption**, ideal for SoC and ASIC applications.

---

## 🎯 Objective

To design a **VLSI-friendly** finite state vending machine controller that is:

- 🧠 **FSM-based**
- 🔋 **Power-efficient**
- 🛠️ Synthesizable (for FPGA or ASIC)
- ⏱️ **Timing-optimized**
- 💾 Area-aware with reduced switching activity

---

## 💡 Key Features

- Accepts coins: ₹1, ₹2, ₹5 (can be parameterized)
- Products: Water, Chips, Soda (example items)
- Returns change if overpaid
- Power-efficient FSM using:
  - **Clock gating**
  - **State encoding optimization**
  - **Glitch-free combinational logic**
- Supports **reset and idle states**
- FSM implemented in **Mealy or Moore** model

---

## 🧰 Tools & Technologies

| Tool               | Purpose                          |
|--------------------|----------------------------------|
| Verilog / VHDL     | RTL Design                       |
| Xilinx ISE / Vivado| Simulation & Synthesis           |
| ModelSim           | RTL Simulation                   |
| Cadence RTL Compiler | Power and timing analysis      |
| GTKWave            | Waveform analysis (Optional)     |

---

## 🧠 FSM Design

| State         | Description                         |
|---------------|-------------------------------------|
| `IDLE`        | Waiting for user input              |
| `COIN_WAIT`   | Accepting coins                     |
| `SELECT_ITEM` | Waiting for item selection          |
| `DISPENSE`    | Dispensing item & calculating change|
| `RETURN_CHANGE` | Return remaining amount           |
| `RESET`       | Returns to idle after timeout       |

---

## ⚙️ RTL Modules

