# AXI NoC UVM Verification

## Project Overview

This project focuses on the implementation and verification of an AXI Network-on-Chip (NoC) architecture using SystemVerilog and UVM.

The design integrates multiple AXI slave interfaces through an AXI NoC interconnect, providing access to multiple memory controllers and embedded memory blocks.

The primary objective is to develop and verify an AXI-based interconnect architecture and explore transaction routing between multiple AXI interfaces and memory subsystems.

## Architecture – Block Diagram

<img width="1155" height="494" alt="Screenshot From 2026-11-25 14-49-13" src="https://github.com/user-attachments/assets/0f89f88a-fd02-4495-b108-dcdd47d18439" />

The following diagram illustrates the overall system architecture implemented in Vivado IP Integrator.

**Architecture Description:**

- **AXI Slave Interfaces:** Four AXI slave interfaces (S00_AXI, S01_AXI, S02_AXI, and S03_AXI) are connected to the AXI NoC.
- **AXI NoC:** The central interconnect responsible for routing AXI transactions between the input interfaces and memory-side interfaces.
- **AXI BRAM Controllers:** Two AXI BRAM controllers provide access to the embedded memory blocks.
- **Embedded Memory:** Two Block RAM (BRAM) instances are connected through the respective AXI BRAM controllers.
- **Clock and Reset:** A simulation clock and reset generator provides the required clock and reset signals for the system.

### AXI NoC Block Design

**Upload your screenshot below this line using GitHub's image upload feature.**

## Design Specifications

| Component | Description |
|---|---|
| Interconnect | AXI Network-on-Chip |
| AXI Slave Interfaces | 4 |
| AXI Master Interfaces | 2 |
| Memory Controllers | 2 AXI BRAM Controllers |
| Memory | Embedded Block RAM |
| Design Environment | Xilinx Vivado |
| RTL Language | SystemVerilog |
| Verification Methodology | UVM |

## System Architecture

The architecture consists of four AXI slave interfaces connected to a centralized AXI NoC interconnect.

The NoC provides two master-side interfaces, which connect to individual AXI BRAM controllers. Each controller provides access to its corresponding embedded memory block.

This architecture provides a platform for exploring multi-interface AXI transaction routing and memory access through a NoC-based interconnect.

## Verification Objectives

The verification environment aims to evaluate the functional behavior of the AXI NoC architecture.

Key verification objectives include:

- AXI read transaction verification.
- AXI write transaction verification.
- Transaction routing through the NoC.
- Multiple AXI interface interactions.
- Memory read and write operations.
- Reset behavior.
- Concurrent transaction handling.
- Functional correctness of the interconnect.

## Tools and Technologies

- **HDL:** SystemVerilog
- **Verification Methodology:** Universal Verification Methodology (UVM)
- **FPGA Design Tool:** Xilinx Vivado
- **Protocol:** AMBA AXI
- **Memory:** Block RAM (BRAM)

## Project Status

Work in progress.

Further development and verification activities are focused on validating AXI transaction handling, interconnect functionality, and memory access behavior.

## Repository

This repository contains the RTL design, verification environment, simulation files, and related project documentation for the AXI NoC UVM verification project.
