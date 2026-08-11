# half-subtractor-
Half Subtractor – Verilog

Description

A Half Subtractor is a combinational logic circuit that subtracts two 1-bit binary numbers and produces two outputs: Difference and Borrow.

⚙️ Inputs and Outputs

Input/Output| Description
A| Minuend
B| Subtrahend
Difference| Result of A − B
Borrow| Borrow generated during subtraction

Truth Table

A| B| Difference| Borrow
0| 0| 0| 0
0| 1| 1| 1
1| 0| 1| 0
1| 1| 0| 0

Logic Equations

- Difference = A XOR B
- Borrow = A' AND B
 Tools Used

- Verilog HDL
- Icarus Verilog / ModelSim / Vivado
- GTKWave (optional)

Simulation

Compile the design and testbench:

iverilog -o half_subtractor_sim half_subtractor.v half_subtractor_tb.v

Run the simulation:

vvp half_subtractor_sim

To view the waveform using GTKWave:

gtkwave half_subtractor.vcd

Expected Result

The simulation verifies all four possible input combinations and confirms that the Difference and Borrow outputs match the Half Subtractor truth table.

 Files

- "half_subtractor.v" – Half Subtractor design
- "half_subtractor_tb.v" – Verilog testbench
- "README.md" – Project documentation
author: Harshitha 