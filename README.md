# Segmented Approximate Adder With Smart Chaining (SASC)

## About The Project

This project focuses on the implementation of an **8-bit Segmented Approximate Adder (SASC)** using **Cadence Virtuoso**. The architecture is inspired by the IEEE paper:

> *Energy-Delay Efficient Segmented Approximate Adder With Smart Chaining*

The proposed design minimizes carry propagation delay and improves energy efficiency using segmented computation and approximate carry prediction techniques.

---

# Motivation

Modern VLSI systems demand:

- High-speed arithmetic circuits
- Low-power operation
- Energy-efficient computation

Traditional Ripple Carry Adders (RCA) suffer from long carry propagation delays.

To overcome this limitation, this project implements a segmented approximate architecture that improves performance with acceptable computational accuracy.

---

# Design Configuration

```text
SASC (8,4,0)
```

| Parameter | Meaning |
|---|---|
| N | Total Adder Bits |
| L | Segment Size |
| C | Truncation Size |

---

# Core Concepts Used

- Approximate Computing
- Ripple Carry Addition
- Carry Prediction
- Smart Carry Chaining
- Segmented Architecture
- Multiplexer-Based Carry Selection

---

# Implemented Modules

## Basic Gates

- AND Gate
- OR Gate
- NOT Gate
- NAND Gate
- NOR Gate
- XOR Gate
- XNOR Gate

## Arithmetic Blocks

- Half Adder
- Full Adder
- 4-bit Ripple Carry Adder

## Approximate Logic Blocks

- Carry Prediction Unit
- 2:1 Multiplexer
- Segmented Adder Block
- 8-bit SASC Adder

---

# Architecture Overview

The 8-bit input operands are divided into two segmented 4-bit blocks.

## Lower Segment

- Computes lower bits
- Generates intermediate carry

## Upper Segment

- Uses carry prediction
- Produces final sum and carry

A smart control signal dynamically selects between accurate and approximate carry paths.

---

# CTRL Signal Operation

| CTRL | Operation Mode |
|---|---|
| 0 | Accurate Mode |
| 1 | Approximate / Fast Mode |

---

# Tools Used

| Software | Purpose |
|---|---|
| Cadence Virtuoso | Schematic Design |
| Spectre Simulator | Circuit Simulation |
| GitHub | Version Control |

---

# Simulation Details

Transient simulations were performed to verify:

- Sum generation
- Carry generation
- CTRL switching operation
- Approximate mode behavior

## Inputs

```text
A<7:0>
B<7:0>
Cin
CTRL
```

## Outputs

```text
Sum<7:0>
Cout
```

---

# Results

The implemented SASC architecture achieved:

- Reduced carry propagation delay
- Faster operation compared to RCA
- Improved energy-delay efficiency
- Functional segmented carry operation

---

# Advantages

- Reduced critical path delay
- Energy-efficient arithmetic architecture
- Scalable segmented structure
- Suitable for approximate computing applications

---

# Applications

- Artificial Intelligence Accelerators
- Image Processing
- DSP Systems
- Multimedia Hardware
- Low-Power Embedded Systems

---

# Repository Structure

```text
SASC_Adder_Project/
│
├── docs/
├── images/
├── report/
└── README.md
```

---

# Future Scope

- 16-bit and 32-bit implementation
- ASIC synthesis
- Layout design
- FPGA implementation
- Advanced Error Recovery Unit (ERU)

---

# Reference

Tayebeh Karimi and Arezoo Kamran,

**“Energy-Delay Efficient Segmented Approximate Adder With Smart Chaining”**

IEEE Transactions on Computers, 2025.

---

# Author

## Shanmugapriya

ECE Student | VLSI Enthusiast
