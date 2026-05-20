# Chipathon 2026  
## " RTL-to-GDSII Design of a Configurable Matrix Accelerator IP on GF180MCU "
---

## Overview

This project focuses on the RTL-to-GDSII implementation of a configurable systolic matrix accelerator IP designed for efficient matrix computations. The design emphasizes scalability, modularity, and ASIC-oriented implementation flow, covering the complete pipeline from RTL design to physical design exploration.

The accelerator is based on a parameterized systolic array architecture, enabling flexible configuration of array dimensions and data widths to explore different performance, area, and power trade-offs.

---

## Objectives

- Design a scalable systolic matrix accelerator IP  
- Develop a modular RTL architecture based on Processing Elements (PEs)  
- Implement a configurable systolic array structure  
- Integrate memory-aware dataflow using SRAM buffering and streaming  
- Build a complete verification environment using testbenches  
- Target a full RTL-to-GDSII ASIC flow using gf180mcu  
- Explore tapeout-ready design practices for chip implementation  
- Validate functionality through FPGA implementation  
---


## System Workflow

1. Input matrices are loaded into on-chip SRAM buffers
2. Data is streamed into the systolic array
3. Each Processing Element performs MAC operations in a pipelined fashion
4. Intermediate results propagate through the array
5. Final outputs are stored in output buffers
6. Results are retrieved through testbench or external interface

---

## Design Constraints

The detailed design constraints, including architecture parameters, memory structure, verification strategy, and ASIC design flow, are documented in:

[Design Constraints](Project%20Proposal/design_constraints.md)

---

## Project Roadmap

The phased development plan is documented separately in:

[Phased Implementation Plan](Project%20Proposal/phased_implementation.md)


---

## Optional Extensions

We plan to integrate a lightweight and an open-source RISC-V Core with our IP if time permits .

---

## Team


| Name                     | GitHub Username | Gmail |
|--------------------------|--------|-------|
| Muhammad Waleed Akram    | Waleed99i    | waleedakram059@gmail.com   |
| Abdul Muiz               | abdmz162    | abdmz.uetian23@gmail.com   |
| Rumali Siddiqua          | Rumali-Siddiqua    | rumalisiddiqua@gmail.com   |

---


## License

Apache License 2.0

---

## Status

Project Proposal in progress .