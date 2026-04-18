# 800V BESS DC-DC Converter

## Overview
This project presents a simulation-based design of a modular 2.5 MW bidirectional DC-DC converter for integrating a high-voltage battery energy storage system (BESS) with an 800V data center HVDC bus.

## Motivation
Modern AI data centers require highly efficient power systems. An 800V DC backbone reduces conversion losses and improves power density, but requires efficient integration with battery storage systems.

## System Architecture
- Modular design: 5 × 500 kW converter modules
- Dual Active Bridge (DAB) topology
- SiC-based switching devices
- High-frequency transformer for galvanic isolation

## Key Features
- Bidirectional power flow (charge/discharge)
- Control modes: Constant Current (CC), Constant Voltage (CV), Constant Power (CP)
- High efficiency target (≥99.5% at full load)
- Scalable modular architecture

## Modeled Performance

| Load | Efficiency |
|------|------------|
| 25%  | 98.7%      |
| 50%  | 99.1%      |
| 75%  | 99.4%      |
| 100% | 99.5%      |

## Calculations
The full efficiency and loss model is provided here:

- `calculations/BESS_DC_DC_Converter_Efficiency_Model.xlsx`

## System Diagram
![Block Diagram](figures/block_diagram.png)

## Project Structure
- `/calculations/` – loss and efficiency modeling
- `/figures/` – system diagrams
- `/sim/` – simulation files

## Note
This is a conceptual and simulation-based design, not a physical prototype.
