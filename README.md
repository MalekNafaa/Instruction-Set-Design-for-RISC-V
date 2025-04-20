# Custom RISC-V ISA Design  

This project focuses on designing a **custom Instruction Set Architecture (ISA)** for a RISC-V CPU, incorporating essential components such as:  

- **Program Counter (PC)**  
- **Arithmetic Logic Unit (ALU)**  
- **Register File**  
- **Control Unit**  
- **Memory Units**  

The custom ISA includes a range of operations—**arithmetic, logical, load/store, and branch instructions**—with detailed documentation on the design, control signals, data flow, and a sample program to demonstrate functionality.  

![CPU Architecture](https://github.com/MalekNafaa/Instruction-Set-Design-for-RISC-V/blob/main/Instruction%20Set%20Design%20for%20RISC-V%20photo.png?raw=true)  

---

## 📜 Supported Instructions  

### **Arithmetic Instructions (R-type)**  
| Instruction | Description |
|-------------|-------------|
| `add`  | Adds the values of two registers and stores the result in a third register. |
| `sub`  | Subtracts the value of one register from another and stores the result in a third register. |

### **Logical Instructions (R-type)**  
| Instruction | Description |
|-------------|-------------|
| `and`  | Performs a bit-wise AND between two registers. |

### **Branch Instructions (B-type)**  
| Instruction | Description |
|-------------|-------------|
| `beq`  | Branches to a specified address if two registers are equal. |
| `blt`  | Branches to a specified address if the first register is less than the second. |

### **Load/Store Instructions (I-type, S-type)**  
| Instruction | Description |
|-------------|-------------|
| `lw`   | Loads a word from memory into a register. |
| `sw`   | Stores a word from a register into memory. |
| `addi` | Adds an immediate value to a register's value and stores the result in the specified register. |

---

## 🖥️ Instruction Format  
All instructions follow **RISC-V standard formats** (R-type, I-type, S-type, B-type), utilizing:  
- **Opcode**  
- **Funct3**  
- **Funct7**  

for proper decoding and execution.  
