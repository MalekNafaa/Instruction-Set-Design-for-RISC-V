This project focuses on designing a custom instruction set architecture (ISA) for a RISC-V CPU, incorporating essential components such as the Program Counter (PC),
Arithmetic Logic Unit (ALU), Register File, Control Unit, and Memory Units.
The custom instruction set design includes a range of operations, including arithmetic, logical, load/store, and branch instructions. The goal is to document the design,
explain the control signals and data flow, and provide a sample program to demonstrate the functionality of the custom RISC-V CPU.
![CPU](https://github.com/MalekNafaa/Instruction-Set-Design-for-RISC-V/blob/main/Instruction%20Set%20Design%20for%20RISC-V%20photo.png?raw=true)


Supported Instructions
The following RISC-V instruction types are supported:

Arithmetic Instructions (R-type):

add: Adds the values of two registers and stores the result in a third register.
sub: Subtracts the value of one register from another and stores the result in a third register.
Logical Instructions (R-type):

and: Performs a logical bit-wise AND operation between the values of two registers.
Branch Instructions (B-type):

beq: Branches to a specified address if the values in two registers are equal.
blt: Branches to a specified address if the value in the first register is less than the value in the second register.
Load/Store Instructions (I-type, S-type):

lw: Loads a word from memory into a register.
sw: Stores a word from a register into memory.
addi: Adds an immediate value to a register's value and stores the result in the specified register.
Instruction Format
Each instruction type adheres to the RISC-V instruction formats (R-type, I-type, S-type, B-type) and utilizes the opcode, funct3, and funct7 fields for decoding.

