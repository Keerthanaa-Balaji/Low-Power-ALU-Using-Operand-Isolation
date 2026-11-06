Low-Power ALU Design Using Operand Isolation Technique
Project Overview
This project focuses on the RTL design and verification of a 4-bit Low-Power Arithmetic Logic Unit (ALU) using the Operand Isolation Technique.

The main objective is to reduce unnecessary switching activity in inactive functional units by isolating their input operands. The design is implemented and simulated using SystemVerilog on EDA Playground.

Operations Supported
Addition
Subtraction
Bitwise AND
Bitwise OR
Tools and Technologies Used
EDA Playground – RTL design and simulation platform
SystemVerilog – Hardware description and verification
Icarus Verilog – RTL simulator
EPWave – Waveform visualization
Project Structure
Low-Power-ALU/
│
├── Normal_ALU/
│   ├── design.sv
│   └── testbench.sv
│
├── Low_Power_ALU/
│   ├── design.sv
│   └── testbench.sv
│
└── README.md
Working Principle
1. Normal ALU
The normal ALU performs arithmetic and logical operations based on the 2-bit select input. Its functional units may experience unnecessary input switching even when they are not selected.

2. Low-Power ALU
The Low-Power ALU uses the Operand Isolation Technique. The input operands are supplied only to the selected functional unit, while the inputs of inactive functional units are forced to zero.

This helps reduce unnecessary switching activity in inactive functional units.

Simulation Results
The design was functionally verified using the following input values:

Operation	Input A	Input B	Expected Output
Addition	5	3	8
Subtraction	5	3	2
AND	5	3	1
OR	5	3	7
Both the Normal ALU and Low-Power ALU produce the expected functional outputs.

Current Project Status
 Normal ALU RTL implementation completed.
 Operand isolation logic implemented.
 Low-Power ALU RTL implementation completed.
 Functional simulation completed.
 Waveform verification using EPWave completed.
 Switching activity comparison pending.
 Quantitative power estimation pending.
Expected Outcome
The Operand Isolation Technique is intended to reduce unnecessary switching activity in inactive ALU functional units while maintaining the same output functionality.

Actual power savings will need to be evaluated through switching activity analysis and power estimation.

Author
ECE Mini Project

Department of Electronics and Communication Engineering
