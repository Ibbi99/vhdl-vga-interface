# vhdl-vga-interface
# VGA Controller in VHDL

This project implements a **VGA signal generator** using VHDL, designed for FPGA deployment. It includes VHDL source code, a constraint file for pin mapping, and a precompiled bitstream for direct use.

---

## Project Structure

```text
vga-controller-vhdl/
├── VGA.vhd      # VHDL source code for VGA signal generation
├── VGA.xdc      # Xilinx Design Constraints file (pin mapping)
└── VGA.bit      # Compiled FPGA bitstream
```
---

## Overview

This VHDL design generates VGA-compatible signals (horizontal sync, vertical sync, RGB outputs) for driving standard VGA monitors. The implementation targets an FPGA board and maps signals using an `.xdc` constraint file.

---

## Features

- Generates 640x480 @ 60Hz VGA output
- Synchronous control of HSYNC and VSYNC
- RGB output signals for basic color patterns or test images
- Modular and synthesizable VHDL code
- Tested and compiled into a `.bit` file

---

## Requirements

- FPGA Development Board (e.g., Xilinx Basys 3 or similar)
- Xilinx Vivado (for synthesis, implementation, and uploading)
- VGA-compatible monitor and cable

---

## Output

The output can be connected to a VGA monitor. The design ensures:
- Correct timing for 640x480 resolution
- Continuous VSYNC and HSYNC pulses
- Simple RGB pattern generation

---

## Future Improvements (Optional)

- Add color gradient or image ROM support
- Implement on-screen text rendering
- Support for higher resolutions
