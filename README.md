
# PipeLined Implementation of MIPS32 Processor

MIPS32 is a **Reduced Instruction Set Architechture (RISC)** which can operate on 32 bits of data at a time.

## Salient Features

### MIPS32 Registers:

* 32, 32 general purpose registers: *R0 to R1*.
* A special purpose register: 32 bit Program Counter pointing to the next instruction to be fetched.


### MIPS Instruction Encoding:
Instructions classified into three groups.
* R-type(Register) : Two Source and One Destination Register.

* I-type(Immediate) : One Source and One Destination Register. 

* J-type(jump) : Not implemented.

 <img width="523" height="233" alt="Image" src="https://github.com/user-attachments/assets/4614a59c-f91e-4610-a7e0-cc65246075c1" />

 ## Pipeline Stages:

 * IF : Instruction Fetch
 * ID : Instruction Decode
 * EX : Execute / Effective Address Calculation.
 * MEM: Memory Access/Branch Completion.
 * WB : Register Write Back

 ### IF Stage :
 $IR <- Mem[PC]$
 $E = MC^2$ 

 ### ID Stage:
 $A  <- Reg[rs]$
 $B  <- Reg[rt]$
 $Imm<- (IR_15)^15##IR_{15-0}$





