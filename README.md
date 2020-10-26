# RISC-V based Microprocessor
RISC-V is a free and open ISA enabling a new era of processor innovation through open standard collaboration. Born in academia and research, RISC-V ISA delivers a new level of free, extensible software and hardware freedom on architecture, paving the way for the next 50 years of computing design and innovation. A number of companies are offering or have already announced RISC-V hardware, open source operating systems with RISC-V support are available and the instruction set is supported in several popular software [toolchains][10].

This repository contains all the information needed to build your RISC-V pipelined core, which has support of base interger RV32I instruction format and testing it with a simple C code using TL-Verilog on [Makerchip IDE platform][9].

[9]:https://www.makerchip.com/
[10]:https://en.wikipedia.org/wiki/Toolchain
# Table of Contents

# Conclusion

This project was done as a part of the RISC-V based MYTH (Microprocessor for You in Thirty Hours) workshop conducted by Kunal Ghosh and Steve Hoover. The current project implements almost the entire RV32I base instruction set. We capable of executing all RISC-V instructions in four cycles with easy pipelining using Transaction-Level Verilog. TL-Verilog not only reduces your code size significantly but allows us to freely declare signals without explicitly declaring them (just like Python does compare to C). In addition, we can generate Verilog/SystemVerilog code from TL-Verilog in Makerchip IDE which using Sandpiper complier. Future work involves modifying the current design to implement support for the remaining operations and also implementation of other standard extensions like M, F and D.

# Acknowledgements
All this wouldn't have been possible without a great set of mentors guiding throughout the workshop, few notable mentions below

* [Kunal Ghosh][1], Co-founder, VSD Corp. Pvt. Ltd.
* [Steve Hoover][2], Founder, Redwood EDA

[1]:https://github.com/kunalg123/ "Kunal Ghosh"
[2]:https://github.com/stevehoover/ "Steve Hoover"

# References
You can follow the below mentioned sites for more information regarding the particular topics.
* RISC-V: https://riscv.org/
* Makerchip Platform: https://makerchip.com/
* TL-Verilog: https://www.redwoodeda.com/tl-verilog or http://tl-x.org/
* Redwood EDA: https://www.redwoodeda.com/
* VLSI System Design: https://www.vlsisystemdesign.com/
