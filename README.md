# FIR-Filter

Company: CODTECH IT SOLUTIONS

Name: Pooja Shukla

Intern ID: CT06DH677

Domain: VLSI

Duration: 6 weeks

Mentor Name: Neela Santosh


DESIGN AND SIMULATE A DIGITAL  FIR (FINITE IMPULSE RESPONSE)  FILTER USING VERILOG
---------------------------------------------------------------------------------------------------------------------------
 ###DESCRIPTION:
 # FIR Filter Design and Simulation Using Verilog

This project presents the design and simulation of a **digital FIR (Finite Impulse Response) filter** using **Verilog Hardware Description Language (HDL)**. The implementation demonstrates how basic DSP (Digital Signal Processing) concepts can be translated into hardware-friendly code, simulated using a testbench, and verified using waveform analysis tools available on **EDA Playground**.

---

## Project Description

A **Finite Impulse Response (FIR) filter** is a fundamental building block in digital signal processing. It is used to filter or process discrete-time signals, attenuating unwanted frequencies while preserving or enhancing desired components. FIR filters are widely preferred due to their inherent **stability**, **linear phase characteristics**, and ease of hardware implementation.

In this project, a **parameterized FIR filter** is implemented using Verilog, allowing for flexible tap sizes and input bit widths. The filter coefficients (also called “taps”) are hard-coded for demonstration purposes, and the design supports signed input data. A corresponding **Verilog testbench** is developed to simulate the filter’s behavior, apply test inputs, and capture output responses over time.

The simulation is performed using **EDA Playground**, a free online IDE for HDL development, which supports tools like ModelSim and Icarus Verilog. The waveform viewer is used to visually inspect the filter’s time-domain response and confirm the correctness of the convolution operation.

---

## Features

- Parameterized number of taps (default: 5)
- Fixed signed filter coefficients: [1, 2, 3, 2, 1]
- Fully synchronous design using clock and reset
- Multiply-accumulate (MAC) architecture
- Shift-register-based sample storage
- Output width extended to accommodate overflow
- Testbench for verification with waveform and terminal output

---

##  Simulation Environment

The testbench performs the following:
- Generates a 100 MHz clock (10 ns period)
- Applies an initial reset signal
- Sends a predefined input sample stream: `[1, 2, 3, 0, -1, 0, 2, 0]`
- Logs each output sample using `$display`
- Optionally displays waveforms for visual analysis

**Expected output** is the convolution result of the input sequence and the coefficient vector, calculated in real-time by the filter module.

---

##  Files in Repository

| File Name         | Description                                 |
|------------------|---------------------------------------------|
| `fir_filter.v`    | Verilog code for the FIR filter             |
| `tb_fir_filter.v` | Testbench for filter simulation             |
| `README.md`       | This documentation file                     |

---


## 🎓 Learning Outcomes

By completing this project, learners will:

- Understand how FIR filters operate in digital signal processing
- Translate mathematical filter equations into Verilog code
- Use shift registers and arithmetic operations in hardware
- Write effective Verilog testbenches
- Use simulation tools and waveform viewers for verification

This project bridges the gap between theoretical DSP knowledge and practical hardware implementation using HDL.


---

