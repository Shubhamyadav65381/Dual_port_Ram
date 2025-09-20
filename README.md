## Dual-Port RAM in Verilog
## Project Overview

This project implements a Dual-Port RAM in Verilog, enabling simultaneous read and write operations on two independent ports. The design supports parameterizable data width, address width, and memory depth, making it flexible for a wide range of digital system applications.

## Key Features

Implementation of a parameterized dual-port RAM.

## Two independent ports:

- Port 0: Supports both read and write.

- Port 1: Supports read-only.

Synchronous write operation triggered on the positive clock edge.

Tri-state outputs when ports are disabled.

Designed in Verilog HDL with a testbench for functional verification.

## Technical Details

## Technology: Verilog HDL

## Target Device: FPGA (generic, synthesis-ready)

## Simulation: Verified using a Verilog testbench.

## Synthesis: Compatible with tools like Xilinx Vivado, ModelSim, or Icarus Verilog.

## Usage

Compile both dual_port_ram.v and test_bench.v using your Verilog simulator (e.g., Icarus Verilog, ModelSim).

Run the testbench to verify read/write operations.

Observe waveforms or console output to confirm correct memory behavior.

For FPGA deployment, include the module in your project and connect it to appropriate logic.

## Project Structure

dual_port_ram.v – Parameterized dual-port RAM module.

test_bench.v – Testbench for simulation and verification.

## Example Operation

The testbench writes values 1 to 16 into the RAM.

Values are then read back simultaneously from both ports, demonstrating independent access.

## Benefits

Flexible, reusable design with configurable parameters.

Demonstrates dual-port memory access for parallel data operations.

Suitable for educational projects, FPGA-based memory design, and digital system prototypes.

## Author

Shubham Yadav

For any questions or support, please feel free to contact the author.
