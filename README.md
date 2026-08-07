# RTL Design – 4-bit Synchronous Up/Down Counter using Verilog HDL

## Project Overview

This project implements a **4-bit Synchronous Up/Down Counter** using **Verilog HDL**. The counter updates its value on every **positive edge of the clock** and counts either upward or downward based on the **up_down** control signal. An **asynchronous reset** is provided to initialize the counter to zero at any time.

The design demonstrates fundamental concepts of **sequential logic**, **counter design**, and **RTL implementation**, making it an excellent beginner-friendly VLSI project.

---

## Block Diagram

The block diagram below illustrates the architecture of the **4-bit Synchronous Up/Down Counter**. The **up_down** control signal determines whether the counter increments or decrements on each positive clock edge. The current count value is stored in a bank of four D Flip-Flops, while the asynchronous reset initializes the counter to **0000** regardless of the clock.


<img width="1536" height="1024" alt="updownbd" src="https://github.com/user-attachments/assets/99b0a566-8357-4228-b471-b4c6e7e4a0f3" />


---

## Features

* 4-bit Synchronous Counter
* Verilog HDL RTL Implementation
* Positive Edge Triggered Design
* Up Counting Mode
* Down Counting Mode
* Asynchronous Reset
* Synthesizable RTL
* Functional Verification using Testbench
* Simulation using EDA Playground

---

## Inputs

| Signal  | Width | Description                          |
| ------- | ----- | ------------------------------------ |
| clk     | 1     | Positive Edge Clock                  |
| rst     | 1     | Asynchronous Active-High Reset       |
| up_down | 1     | Direction Control (1 = Up, 0 = Down) |

---

## Output

| Signal | Width | Description          |
| ------ | ----- | -------------------- |
| count  | 4     | 4-bit Counter Output |

---

## Functional Operation

| Reset | Up_Down | Operation             |
| ----- | ------- | --------------------- |
| 1     | X       | Counter Reset to 0000 |
| 0     | 1       | Counter Increments    |
| 0     | 0       | Counter Decrements    |

---

## Working Principle

* The counter updates only on the **rising edge of the clock**.
* When **up_down = 1**, the counter increments by one.
* When **up_down = 0**, the counter decrements by one.
* The **asynchronous reset** immediately clears the counter to **0000**, independent of the clock.
* The current count value is continuously fed back to generate the next count value.

---

## Project Structure

```text
RTL-Design-4bit-UpDown-Counter/
│
├── up_down_counter.v
├── up_down_counter_tb.v
├── block_diagram.png
└── README.md
```

---

## Verification

The design was verified using a dedicated Verilog testbench covering:

* Asynchronous Reset
* Up Counting Sequence
* Down Counting Sequence
* Mode Switching
* Multiple Clock Cycles
* Functional Verification

The simulation confirms correct counter operation in both counting modes.

---

## Applications

* Digital Timers
* Event Counters
* Frequency Division
* Address Generation
* Embedded Systems
* FPGA Designs
* ASIC RTL Design
* Digital Control Systems

---

## Tools Used

* Verilog HDL
* EDA Playground
* Icarus Verilog
* EPWave
* GitHub

---

## Learning Outcomes

This project strengthened my understanding of:

* RTL Design
* Sequential Logic Circuits
* Counter Design
* Verilog HDL Coding
* Clocked Sequential Systems
* Asynchronous Reset Logic
* Functional Verification
* Testbench Development
* Digital System Design

---

## Future Improvements

* Parameterizable Counter Width
* Synchronous Enable Signal
* Loadable Counter
* Overflow and Underflow Detection
* Terminal Count Output
* Clock Enable Support
* SystemVerilog Assertions (SVA)
* UVM-based Verification

---

## Author

**Dikshitha M**

Aspiring RTL Design Engineer | VLSI Enthusiast

💼 **LinkedIn:**
https://www.linkedin.com/in/dikshitha-m-34355b308/

⭐ If you found this project useful, consider giving this repository a star!


