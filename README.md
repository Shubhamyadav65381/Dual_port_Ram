## Dual-Port RAM in Verilog
![Block Diagram]([[dual_port_ram_diagram.png_](https://github.com/Shubhamyadav65381/Dual_port_Ram/blob/main/output%20waveform.png?raw=true](https://github.com/Shubhamyadav65381/Dual_port_Ram/blob/main/RTL.png?raw=true)))

## Table of Contents
Project Overview

- Key Features

- Visual Overview

- Technical Details

- Usage Instructions

- Project Structure

- Example Operation

- Benefits

- Contributing

- License

- Author & Contact

## Project Overview
This project implements a Dual-Port RAM module in Verilog, allowing for simultaneous read and write operations on two independent ports. The design is parameterizable for data width, address width, and memory depth, making it suitable for a wide range of digital systems.

## Key Features
- Fully parameterized dual-port RAM design

Two independent ports:

- **Port 0:** Read and Write support

- **Port 1:** Read-only support

Synchronous write operation (positive clock edge)

Tri-state outputs when ports are disabled

Developed in Verilog HDL along with a complete testbench for verification

## Visual Overview
![RAM Architecture]( architecture of the dual-port RAM*

## Technical Details
**Technology:** Verilog HDL

**Target Device:** FPGA (synthesis-ready, device-agnostic)

**Simulation:** Functional verification using a Verilog testbench

Synthesis Tools Supported: Xilinx Vivado, ModelSim, Icarus Verilog

## Usage Instructions
- Compile

bash
- verilog dual_port_ram.v test_bench.v -o ram_tb
- Run the Testbench

bash
- vvp ram_tb
- Verify Results

- Check simulation waveforms 

- Review console output for correct read/write operation

## FPGA Deployment

- Include dual_port_ram.v in your synthesizable project.

- Connect module ports to the appropriate top-level logic as per system requirements.

## Project Structure
text

.

├── dual_port_ram.v                       # Parameterized dual-port RAM module 

├── test_bench.v                          # Testbench for simulation and verification

├── dual_port_ram_diagram.png             # Block diagram image

├── simulation_waveform.png               # Waveform from simulation

├── ram_architecture.png                  # Architecture illustration

└── README.md                             # Project documentation

## Example Operation
- The testbench writes sequential values (1–16) into the RAM.

- Values are read back simultaneously from both ports to demonstrate independent, parallel access.

Benefits
- Highly flexible and reusable module with configurable parameters

- Demonstrates industry-standard dual-port memory access for parallel read/write

- Suitable for teaching, prototype FPGA projects, and real-world digital system designs.

## Contributing
- Contributions and suggestions are welcome!
- Feel free to submit issues or pull requests for improvements.

## Author & Contact
Shubham Yadav
For support or questions, please open an issue on this repository or contact via GitHub.
