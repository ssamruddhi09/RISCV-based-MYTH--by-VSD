# Application Binary Interface (ABI)

## Overview

The **Application Binary Interface (ABI)** defines how application programs communicate with the operating system and hardware at the binary level. It specifies register usage, calling conventions, and system call interactions.

---

## ABI in System Architecture

ABI acts as a bridge between software and hardware. Applications interact with standard libraries and the operating system, which then communicates with hardware using ISA and ABI conventions.

<img width="1843" height="1014" alt="1" src="https://github.com/user-attachments/assets/ee9ce33b-2667-48b5-b124-1bf343149cb6" />


---

## Registers and Memory Representation

RISC-V uses general-purpose registers for computation and data transfer.

- RV32 → 32-bit registers  
- RV64 → 64-bit registers (XLEN = 64)  
- RISC-V follows **little-endian memory addressing**

<img width="1818" height="1113" alt="3" src="https://github.com/user-attachments/assets/294469b3-9537-4804-a568-bb18ef40c436" />


---

## RISC-V Instruction Formats <img width="1818" height="1113" alt="3" src="https://github.com/user-attachments/assets/294469b3-9537-4804-a568-bb18ef40c436" />


RISC-V instructions follow standard formats that define how operands and operations are encoded.

### R-Type
Used for register-to-register operations.

### I-Type
Used for immediate and load instructions.

### S-Type
Used for store instructions.

<img width="1782" height="1088" alt="4" src="https://github.com/user-attachments/assets/fec0a93f-65a4-4d0d-ad1b-81d33870af53" />

---


## ABI Register Convention

RISC-V defines 32 registers (x0 – x31) with specific roles.

| Register | Usage |
|-----------|------------|
| x0 | Constant zero |
| x1 | Return address |
| x2 | Stack pointer |
| x5-x7 | Temporary registers |
| x8-x9 | Saved registers |
| x10-x17 | Function arguments |
| x18-x27 | Saved registers |
| x28-x31 | Temporary registers |

<img width="1782" height="1092" alt="5" src="https://github.com/user-attachments/assets/aa3679b3-a689-40c2-8c86-42f94afead9e" />

---

## Summary

- ABI connects software and hardware  
- Defines register roles and calling conventions  
- Helps in instruction execution and memory interaction  
