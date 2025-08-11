# ECHO2ME USB Audio Interface

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![KiCad](https://img.shields.io/badge/KiCad-9.0-green.svg)
![Status](https://img.shields.io/badge/status-prototype-orange.svg)

## Overview

ECHO2ME is an open-source USB audio interface designed specifically for bass guitar recording. Inspired by commercial interfaces like the Focusrite Scarlett Solo and Behringer UMC series, this project aims to create a more portable, casual, and affordable alternative.

## Features

- **High-impedance input** (1MΩ) suitable for passive bass pickups
- **Variable gain preamp** (0-40dB)
- **USB-powered** - no external power supply needed
- **24-bit/48kHz** audio quality (PCM2902C)
- **Compact design** - perfect for mobile recording
- **Total cost**: Under $30 in components

## Motivation

After using various commercial audio interfaces, I wanted something:
- More portable than desktop interfaces
- Cheaper than commercial options
- Designed specifically for bass guitar
- Easy to build and modify

## Technical Specifications

### Analog Board
- Input impedance: 1MΩ
- Gain range: 0-40dB (adjustable)
- Frequency response: 20Hz-20kHz (±0.1dB)
- THD: <0.01% @ 1kHz
- Power: ±15V (from power board)

### USB Board
- ADC/DAC: PCM2902C
- Resolution: 16-bit
- Sample rates: 32kHz, 44.1kHz, 48kHz
- USB: Full-speed USB 1.1/2.0 compatible
- Driver: USB Audio Class 1.0 (no drivers needed)

## Repository Structure

- `/hardware` - KiCad design files
- `/documentation` - Schematics, assembly guides, design documentation
- `/software` - Test scripts and utilities
- `/bom` - Bill of materials
- `/images` - Photos and renders
- `/releases` - Production-ready files

## Getting Started

### Required Tools
- KiCad 9.0 or later
- Basic soldering equipment
- Multimeter for testing

### Building the Interface

1. **Order PCBs**
   - Upload gerber files from `/releases` to JLCPCB
   - 2-layer boards, 1.6mm thickness, HASL finish

2. **Order Components**
   - See BOM files in `/bom` directory
   - Recommended suppliers: Mouser, DigiKey

3. **Assembly**
   - Start with SMD components (if any)
   - Install ICs last
   - See assembly guides in `/documentation`

### Quick Start Guide

1. Clone this repository
2. Open KiCad projects in `/hardware`
3. Review schematics and PCB layouts
4. Generate gerbers or use pre-made ones in `/releases`
5. Order PCBs and components
6. Assemble and test

## Design Philosophy

The design prioritizes:
- **Simplicity**: Easy to understand and modify
- **Quality**: Professional-grade audio performance
- **Affordability**: Common, inexpensive components
- **Repairability**: Through-hole components where possible

## Current Status

- [x] Schematic design complete
- [x] PCB layout complete
- [x] Prototype ordered from JLCPCB
- [ ] First prototype assembly
- [ ] Testing and validation
- [ ] Revision 2 based on testing

## Contributing

Contributions are welcome! Please feel free to:
- Report bugs
- Suggest improvements
- Submit pull requests
- Share your builds

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- KiCad community for the excellent EDA software
- JLCPCB for affordable PCB manufacturing
- Texas Instruments for the PCM2902C datasheet and reference design

## Contact

- GitHub Issues: For bug reports and feature requests
- Discussions: For general questions and show-and-tell

---
*Made with ❤️ for the DIY audio community*
