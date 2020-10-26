# RISC-V based Microprocessor
RISC-V is a free and open ISA enabling a new era of processor innovation through open standard collaboration. Born in academia and research, RISC-V ISA delivers a new level of free, extensible software and hardware freedom on architecture, paving the way for the next 50 years of computing design and innovation. A number of companies are offering or have already announced RISC-V hardware, open source operating systems with RISC-V support are available and the instruction set is supported in several popular software [toolchains][10].

This repository contains all the information needed to build your RISC-V pipelined core, which has support of base interger RV32I instruction format and testing it with a simple C code using TL-Verilog on [Makerchip IDE platform][9].

[9]:https://www.makerchip.com/
[10]:https://en.wikipedia.org/wiki/Toolchain

# Table of Contents
* [Introduction to RISC-V ISA](#Introduction-to-RISC-V-ISA)
* RISCV TOOL CHAIN
* Introduction to ABI 
* Digital Logic with TL-Verilog and Makerchip
* Basic RISC-V CPU micro-architecture
    * Instruction Fetch and Decode
    * Register File Read and Write
   ALU and Control Logic
* Pipelined RISC-V CPU
    * Pipelining the CPU
    * Completing the RISC-V CPU
* Conclusion
* Acknowledgements
* References

## Introduction to RISC-V ISA
An Instruction Set Architecture (ISA) defines, describes, and specifies how a particular computer processor core works. The ISA describes the registers and describes each machine-level instruction. The ISA forms the interface between hardware and software. Hardware engineers design digital circuits to implement a given ISA specification. Software engineers write code (operating systems, compilers, etc.) based on a given ISA specification.


A RISC-V ISA is defined as a base integer ISA, which must be present in any implementation, plus optional extensions to the base ISA. Each base integer instruction set is characterized by

1. Width of the integer registers (XLEN)
2. Corresponding size of the address space
3. Number of integer registers (32 in RISC-V)

More details on RISC-V ISA can be obtained [here].
# RISCV TOOL CHAIN
# Introduction to ABI and RISC-V specifications

System programming involves designing and writing computer programs that allow the computer hardware to interface with the programmer and the user, leading to the effective execution of application software on the computer system. In order to achieve systems programming there needs to be an interface which communicates between software and hardware which is where the APPLICATION BINARY INTERFACE comes into play.
# Digital Logic with TL-Verilog and Makerchip
# Basic RISC-V CPU micro-architecture
# Pipelined RISC-V CPU

# Conclusion

This project was done as a part of the [RISC-V based MYTH (Microprocessor for You in Thirty Hours)][3] workshop conducted by Kunal Ghosh and Steve Hoover. The current project implements almost the entire RV32I base instruction set. We capable of executing all RISC-V instructions in four cycles with easy pipelining using Transaction-Level Verilog. TL-Verilog not only reduces your code size significantly but allows us to freely declare signals without explicitly declaring them (just like Python does compare to C). In addition, we can generate Verilog/SystemVerilog code from TL-Verilog in Makerchip IDE which using Sandpiper complier. Future work involves modifying the current design to implement support for the remaining operations and also implementation of other standard extensions like M, F and D.

[3]:https://www.vlsisystemdesign.com/riscv-based-myth/
# Acknowledgements
All this wouldn't have been possible without a great set of mentors guiding throughout the workshop, few notable mentions below

* [Kunal Ghosh][1], Co-founder, VSD Corp. Pvt. Ltd.
* [Steve Hoover][2], Founder, Redwood EDA

[1]:https://github.com/kunalg123/ "Kunal Ghosh"
[2]:https://github.com/stevehoover/ "Steve Hoover"

# References
You can follow the below mentioned sites for more information regarding the particular topics.
* [RISC-V][21]
* [Makerchip Platform][22]
* [TL-Verilog][23]
* [Redwood EDA][24]
* [VLSI System Design][25]

[21]:https://riscv.org/
[22]:https://makerchip.com/
[23]:https://www.redwoodeda.com/tl-verilog 
[24]:https://www.redwoodeda.com/
[25]:https://www.vlsisystemdesign.com/
