# Simple and Affordable Linear Power Supply (0-30V, 0-3A)

This repository accompanies a video about this power supply: https://youtu.be/LigN5W8R_zc

## Disclaimer

This design is provided for educational and DIY purposes. Building a linear power supply involves potentially hazardous voltages and significant heat dissipation. Ensure that the transformer, rectifier, pass transistors, heatsinks, wiring, fusing, and enclosure are appropriately rated for your intended application.

Always take appropriate electrical safety precautions when building and testing the power supply.

This LPS is based on **Simple and Affordable Power Supply v17**: https://forum.cxem.net/topic/76820-%D0%BF%D1%80%D0%BE%D1%81%D1%82%D0%BE%D0%B9-%D0%B8-%D0%B4%D0%BE%D1%81%D1%82%D1%83%D0%BF%D0%BD%D1%8B%D0%B9-%D0%B1%D0%BF-050-%D0%B2/

My version is designed for an adjustable output voltage of **0-30 V** and an output current of **0-3 A**. However, the design can be easily adapted to achieve significantly higher output voltage and current ratings, depending on the transformer, power components, cooling, and other design considerations.

## Features

- **Constant Voltage (CV) mode** - regulates the output voltage.
- **Constant Current (CC) mode** - regulates the output current.
- **Latching overcurrent protection** - shuts down the output when an overcurrent condition occurs and remains latched until reset.
- **Overtemperature protection (OTP)** - protects the power supply against excessive temperature.
- **Transformer tap selector** - selects the appropriate transformer winding tap to improve efficiency and reduce power dissipation.
- **Four-layer PCB** - a four-layer printed circuit board designed to accommodate the circuit and its layout requirements.

## Important Note on Circuit Stability

The circuit may be prone to oscillation if inappropriate compensation capacitors are used around the operational amplifiers. The values and placement of these capacitors are important for ensuring stable operation.
Do not change the compensation capacitor values without carefully evaluating circuit stability. If modifying the design, verify its behavior under different operating conditions and loads, preferably using an oscilloscope.

## Project Files

This repository includes the KiCad project files:

- `.kicad_pro` - project configuration.
- `.kicad_sch` - schematic.
- `.kicad_pcb` - PCB layout.

and Gerber files: `Gerber.zip`
