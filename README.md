\# Energy-Delay Efficient Segmented Approximate Adder (SASC)



\## Overview

This project implements an 8-bit Segmented Approximate Adder (SASC) based on the IEEE paper:



"Energy-Delay Efficient Segmented Approximate Adder With Smart Chaining"



The design was implemented using Cadence Virtuoso.



\---



\## Features

\- Segmented Ripple Carry Adder

\- Carry Prediction Logic

\- Smart Carry Chaining

\- Approximate Computing

\- Reduced Delay

\- Reduced Energy Consumption



\---



\## Tools Used

\- Cadence Virtuoso

\- Spectre Simulator

\- Verilog Concepts

\- Linux/Unix Environment



\---



\## Project Structure

\- docs/

\- report/

\- images/



\---



\## Results

\- Successful transient simulation

\- Functional Sum and Cout outputs

\- CTRL-based operation verified



\---

## Project Highlights

- Designed an 8-bit Segmented Approximate Adder (SASC)
- Implemented using Cadence Virtuoso
- Reduced carry propagation delay using segmented architecture
- Implemented carry prediction and smart chaining logic
- Verified functionality using transient simulations
- Compared approximate and accurate operating modes using CTRL signal

---

## Architecture

The adder is divided into segmented 4-bit blocks. Carry prediction logic and smart chaining improve speed and reduce energy consumption.

Configuration Used:

SASC (8,4,0)

Where:
- N = Total bits
- L = Segment size
- C = Truncation size

---

## Applications

- Artificial Intelligence Hardware
- DSP Systems
- Image Processing
- Multimedia Systems
- Low-Power VLSI Systems



\## Author

Shanmugapriya

