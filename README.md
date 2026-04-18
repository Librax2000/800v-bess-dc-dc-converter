# 800V BESS DC-DC Converter

## Overview

This project presents a simulation-based design of a modular 2.5 MW bidirectional DC-DC converter for integrating a high-voltage battery energy storage system (BESS) with an 800V data center HVDC bus.

## Motivation

Modern AI data centers require highly efficient power systems. An 800V DC backbone reduces conversion losses and improves power density, but requires efficient integration with battery storage systems.

## Why This Matters

Modern data centers are shifting toward high-voltage DC (HVDC) architectures to improve efficiency and reduce power conversion stages.

This project demonstrates how a modular bidirectional DC-DC converter enables:

* Efficient integration of battery storage systems
* Reduced transmission losses at higher voltages (800V)
* Scalable power delivery for AI and high-performance computing loads

The design highlights how advanced power electronics (SiC + DAB topology) can push efficiencies above 99%.

## System Architecture

* Modular design: 5 × 500 kW converter modules
* Dual Active Bridge (DAB) topology
* SiC-based switching devices
* High-frequency transformer for galvanic isolation

**Total system power: 2.5 MW across 5 modular converter units**

## Key Features

* Bidirectional power flow (charge/discharge)
* Control modes: Constant Current (CC), Constant Voltage (CV), Constant Power (CP)
* High efficiency target (≥99.5% at full load)
* Scalable modular architecture

## Modeled Performance

| Load | Efficiency |
| ---- | ---------- |
| 25%  | 98.7%      |
| 50%  | 99.1%      |
| 75%  | 99.4%      |
| 100% | 99.5%      |

## Calculations

The full efficiency and loss model is provided here:

* `calculations/BESS_DC_DC_Converter_Efficiency_Model.xlsx`

## System Architecture Diagram

![Block Diagram](figures/block_diagram.png)

[Download high-quality PDF](figures/block_diagram.pdf)

## Project Structure

* `/calculations/` – loss and efficiency modeling
* `/figures/` – system diagrams
* `/sim/` – simulation files

## Future Work

* Detailed switching loss modeling using real SiC device data
* Thermal analysis of converter modules
* Control strategy implementation (phase-shift control for DAB)
* Hardware prototyping of a scaled-down system

## Note

This is a conceptual, simulation-based power electronics design intended to demonstrate system-level architecture and efficiency trends.
