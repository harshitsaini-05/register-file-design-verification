# register-file-design-verification
# Design and Verification of a 4-Bit Register File with Multiport Read and Write Support

# Project Overview

This project focuses on the design and verification of a **4-bit register file** with **multiport read and write capabilities** using **SystemVerilog HDL**.
A register file is a fundamental component in digital systems such as CPUs, allowing fast storage and retrieval of data.

The design supports **simultaneous read and write operations**, making it efficient for high-performance digital architectures.

---

# Objectives

* Design a 4-bit wide register file using SystemVerilog
* Implement multiport read and write functionality
* Ensure synchronous operation using clock signals
* Verify the design using a comprehensive testbench
* Analyze simulation results through waveform outputs

---

# Features

*  4-bit data width
*  Multiple read ports
*  Single/Multiple write support (based on design)
*  Addressable registers
*  Synchronous write operation
*  Fast parallel read access
*  Fully verified using testbench

---

# Design Details

The register file consists of:

* A set of registers (memory elements)
* Read ports (for fetching data)
* Write port (for updating data)
* Address lines to select registers
* Control signals like:

  * `clk` (clock)
  * `we` (write enable)
  * `read_addr`
  * `write_addr`

# Working Principle

* Data is written into the register on the rising edge of the clock when write enable is active
* Multiple registers can be accessed simultaneously through different read ports
* Output is updated based on selected read addresses

---

# Verification

A dedicated **testbench** is created to verify the functionality:

* Applies different input combinations
* Tests read/write operations
* Checks edge cases
* Generates waveform outputs

Simulation ensures:

* Correct data storage
* Accurate read operations
* Proper synchronization with clock

---

# Simulation & Waveform Analysis

* Simulation performed using tools like:

  * ModelSim / QuestaSim
  * EDA Playground

Waveforms are analyzed to verify:

* Timing correctness
* Data integrity
* Control signal behavior

---

##Tools & Technologies

* **SystemVerilog HDL**
* **ModelSim **
* **Digital Design Concepts**

---

# Project Structure

```
├── design.sv          # Register file design
├── testbench.sv       # Testbench for verification
├── waveform.vcd       # Simulation waveform (optional)
└── README.md          # Project documentation
```

---

# Applications

* CPU register files
* Microprocessors and microcontrollers
* Embedded systems
* Digital signal processing systems

---

# Future Enhancements

* Increase register size (8-bit / 16-bit)
* Add more read/write ports
* Implement pipelining
* Add error detection mechanisms


---

# Conclusion

This project demonstrates the fundamental concepts of **register file design and verification**, highlighting the importance of multiport access in modern digital systems. It strengthens understanding of memory structures, timing behavior, and hardware verification techniques.

---
