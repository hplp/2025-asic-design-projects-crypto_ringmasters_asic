# Project_Template

## Team Name: 
Crypto_Ringmasters

## Team Members:
- Shafat Shahnewaz
- Rumali Siddiqua

## Project Title:
ASIC Implementation of a Ring Oscillator-Based PUF on TinyTapeout10

## Project Description:
This proposal details the design, implementation, and verification of an ASIC-based Ring Oscillator
 Physical Unclonable Function (RO-PUF) using the TinyTapeout 10 digital flow and the Sky130 Process
 Design Kit (PDK). Building on our prior FPGA work, our design is implemented in synthesizable Verilog
 and integrated into the TT10. The goal is to generate a tapeout-ready GDSII file while ensuring high
 entropy and reliable security metrics through rigorous RTL simulation, synthesis, place-and-route, and
 post-layout verification.

## Key Objectives:
- Develop a synthesizable RO-PUF design featuring Ring Oscillator Module, Frequency Counter, Comparator and Control Logic, Control FSM.

- Integrate the design into the TinyTapeout 10 flow by adapting the TT10 Verilog template
 and updating configuration files for correct pin mappings and design parameters.
 
- Perform comprehensive verification: Execute pre-synthesis simulation, synthesis using Yosys
 (with the Sky130 PDK), place-and-route via OpenROAD, DRC/LVS with Magic/KLayout, and
 post-layout timing simulations with parasitic extraction.

## Technology Stack:
RTL Development & Simulation: Verilog, Icarus Verilog/Verilator, GTKWave.

Synthesis: Yosys with the Sky130 PDK.

Place & Route: OpenROAD.

Layout Verification: Magic and/or KLayout.

Version Control and Documentation: Git and LaTeX.

## Expected Outcomes:
- A fully verified ASIC RO-PUF design integrated within the TinyTapeout 10 flow.
- Detailed simulation, synthesis, and timing reports that validate design performance and security

## Tasks:

| Task                         | Description                                                                                      | Assigned To       |
|------------------------------|--------------------------------------------------------------------------------------------------|-------------------|
| Environment Setup            | Clone TT10 repo, organize modules, and configure pin mapping                                    | Shafat & Rumali   |
| RTL Design                   | Implemented ring oscillator, frequency counter, comparator, and FSM in synthesizable Verilog      | Shafat & Rumali           |
| Functional Verification      | Develop testbenches and validate PUF bit generation using simulations                           | Shafat & Rumali            |
| Synthesis & Optimization     | Run Yosys synthesis with Sky130 PDK, apply constraints, and optimize logic                      |             |
| Place & Route & DRC/LVS      | Use OpenROAD, Magic, and KLayout for layout and design checks                                   |             |
| Post-Layout Simulation       | Extract parasitics, perform post-layout timing verification                                     |             |
| Documentation & Signoff     | Write report, generate GDSII, summarize results                                                 | Both              |


## Timeline:

| Milestone                        | Timeline |
|----------------------------------|----------|
| Functional Simulation and Verification | Week 1  |
| Synthesis and Early Optimization      | Week 2  |
| Place & Route and Layout Verification | Week 3  |
| Post-Layout Simulation and Final Signoff | Week 4  |

