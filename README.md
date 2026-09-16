# 11-bit DAC Design and Implementation in Cadence Virtuoso

## Overview

This project presents the design and functional verification of an 11-bit Digital-to-Analog Converter (DAC) implemented in Cadence Virtuoso.

The DAC architecture is based on a research-paper-derived 3-bit sub-DAC structure and combines segmented DAC sections to achieve the required 11-bit resolution.

## Architecture

The DAC consists of:

- 3-bit sub-DAC section based on the reference architecture
- 5-bit binary-weighted DAC section for the LSB portion
- Integration of the sub-DAC sections to form the complete 11-bit DAC
- Differential output structure
- Control logic implemented using Verilog-A components where required

## Current Implementation

The current stage focuses on ideal-component-level architecture verification.

### Completed

- Implemented the 3-bit sub-DAC architecture
- Implemented the 5-bit LSB DAC section
- Integrated the sections into an 11-bit DAC
- Developed simulation testbenches
- Performed transient simulations
- Verified DAC output levels and functional behavior
- Organized the Cadence project for further transistor-level implementation

### Future Work

- MOS transistor-level implementation
- Pre-layout simulation
- Layout implementation
- DRC and LVS verification
- Post-layout simulation
- PVT and corner analysis
- Monte Carlo analysis
- Performance evaluation including INL, DNL, settling time and other DAC parameters

## Tools and Technology

- Cadence Virtuoso
- Spectre Simulator
- GPDK90 CMOS technology
- Verilog-A
- Git / GitHub

## Project Structure

```text
arch_verify/
├── 3-bit DAC
├── 5-bit DAC
├── 11-bit DAC
├── Testbenches
└── Verilog-A components
