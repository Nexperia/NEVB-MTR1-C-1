<picture align="center">
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Nexperia/NEVC-MCTRL-100-t01/main/docs/img/nexperia_logo_white.svg">
  <img alt="Nexperia Logo" src="https://www.nexperia.com/.resources/nexperia-theme/images/logo.png">
</picture>

-----------------
# NEVB-MTR1-C-1: Motor Controller Board Hardware Design Files

![Revision](https://img.shields.io/badge/Version-1.0-blue) [![License - MIT/X Consortium](https://img.shields.io/badge/License-MIT%2FX%20Consortium-green)](https://github.com/Nexperia/NEVB-MTR1-C-1/blob/main/LICENSE)

## Introduction

This repository contains the hardware design files for the NEVB-MTR1-C-1 Motor Controller Board, a key component of Nexperia's Motor Evaluation Kit NEVB-MTR1-KIT1. The controller board serves as the central unit for motor control operations, interfacing between the microcontroller (Arduino Leonardo) and the 3-Phase Inverter Board.

The NEVB-MTR1-KIT1 evaluation kit includes:

- **Motor Controller Board (NEVB-MTR1-C-1)**: The central unit for motor control operations (this repository).
- **3-Phase Inverter Board (NEVB-MTR1-I56-1)**: The main powerstage for driving the motor.
- **Leonardo R3 Development Board**: Acts as the core microcontroller platform for the system.
- **3-Phase BLDC Motor with Hall Sensors**: The motor that is directly controlled by the system.
- Additional screws, plugs, and tools necessary for setup and operation.

## Schematics

The controller board design is organized into hierarchical schematic sheets:

![Main Schematic](drawings/nevb_mtr1_c_1.svg)

![DC-DC Converter](drawings/nevb_mtr1_c_1-DC-DC%20converter.svg)

![Microcontroller](drawings/nevb_mtr1_c_1-Microcontroller.svg)

![User Inputs](drawings/nevb_mtr1_c_1-User%20inputs.svg)

![Gate Drivers](drawings/nevb_mtr1_c_1-Gate%20Drivers.svg)

![Back EMF Sense](drawings/nevb_mtr1_c_1-Back%20EMF%20sense.svg)

![Fault Reporting](drawings/nevb_mtr1_c_1-Fault%20Reporting.svg)

![Hardware and Notes](drawings/nevb_mtr1_c_1-Hardware%20and%20notes.svg)

## Bill of Materials

An interactive Bill of Materials (iBOM) is available in the `bom/` directory. Open `bom/ibom.html` in a web browser to view component placement, reference designators, and sourcing information. The BOM is also available in CSV format at `bom/nevb_mtr1_c_1.csv`.

## Manufacturing Files

Gerber files for PCB manufacturing are located in the `gerbers/` directory.

## Design Software

This board was designed using [KiCad](https://www.kicad.org/) EDA software (version 9.0 or newer recommended).

To open and edit the design:

1. Install KiCad from [https://www.kicad.org/download/](https://www.kicad.org/download/)
2. Open the project file: `nevb_mtr1_c_1.kicad_pro`

## Related Repositories

- **Firmware**: [NEVC-MTR1-t01](https://github.com/Nexperia/NEVC-MTR1-t01) - Trapezoidal control firmware for the evaluation kit

## Safety Precautions

When working with these hardware designs, exercise caution with high-voltage components and follow proper ESD, assembly, and testing procedures.

## Contributing

Contributions to improve the hardware design are welcome. To contribute:

- Fork the repository.
- Create a new branch for your feature or fix.
- Commit your changes with clear documentation.
- Push to your branch and submit a pull request.

## License

This project is licensed under the MIT/X Consortium License, a permissive free software license. For more details on the MIT/X Consortium License, please refer to the LICENSE file included in this repository.
