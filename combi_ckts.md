# Combinational Logic Labs – Makerchip and TL-Verilog

This document records implementation and verification of combinational logic circuits using the Makerchip platform and TL-Verilog.

---

## 1. Full Adder

### Theory

A Full Adder is a combinational circuit that adds three input bits:

- A  
- B  
- Carry Input (Cin)  

It produces two outputs:

- Sum (S)  
- Carry Output (Cout)  

---

### Boolean Expressions

Sum = A ⊕ B ⊕ Cin
Cout = (A · B) + (Cin · (A ⊕ B))


---

### Full Adder Logic Circuit

<img width="1339" height="737" alt="full adder" src="https://github.com/user-attachments/assets/fa3a0d10-6c51-4834-ae09-454306d1c551" />


---

### Cascaded Full Adders (Multi-bit Addition)

Multiple Full Adders can be connected together to perform binary addition of multi-bit numbers. This configuration is known as a Ripple Carry Adder.

<img width="1728" height="756" alt="fulladder1 0" src="https://github.com/user-attachments/assets/090683a9-aa12-491e-9d3a-1b471220d818" />

---

### Observations


- XOR gates generate the Sum output  
- Carry output is generated using AND-OR logic  
- Cascading Full Adders introduces propagation delay  

---

## 2. Multiplexer (MUX) Lab

### Objective

To implement and verify a 2:1 multiplexer using TL-Verilog in Makerchip.

---

### MUX Logic

A multiplexer selects one input based on a select signal.

$out = $sel ? $in1 : $in2

---

### MUX Concept Diagram (Lab Work)

<img width="1689" height="981" alt="mux" src="https://github.com/user-attachments/assets/999d3a79-2e15-4295-8b69-fcdc0e162088" />

---

### TL-Verilog Implementation in Makerchip &  Waveform Verification

<img width="1915" height="929" alt="simple_mux_code" src="https://github.com/user-attachments/assets/86018756-9240-415d-89b5-1ffbe89d4d61" />


---


### Observations

- Output follows the selected input  
- Select signal controls the data path  
- Waveform confirms correct logical behavior  

---

## 3. Vector Operations Lab

### Objective

To perform arithmetic operations on multi-bit vectors using TL-Verilog.

---

### Concept

Vectors allow operations on multiple bits simultaneously.

Example:
$out[4:0] = $in1[3:0] + $in2[3:0]


This produces a 5-bit output from two 4-bit inputs.

---

### Vector Concept Diagram (Lab Work)

<img width="1667" height="956" alt="vectors" src="https://github.com/user-attachments/assets/901a6764-247d-4294-ad00-767272f21325" />

---


### TL-Verilog Vector Implementation & Waveform Verification

<img width="1915" height="917" alt="vector_code" src="https://github.com/user-attachments/assets/3d8bbbe2-96de-451d-9170-f9aaf4802625" />


---

### Observations

- Arithmetic operators treat vectors as binary numbers  
- Output width increases to include carry bit  
- Vector operations simplify multi-bit arithmetic design  

---

## Tools Used

- Makerchip IDE  
- TL-Verilog  
- Verilator Simulator  
- Waveform Viewer  

---

## Key Learnings

- Understanding combinational circuit design  
- Implementation of logic using TL-Verilog  
- Simulation-based verification of circuits  
- Performing arithmetic operations using vectors  

---

## Conclusion

These labs demonstrate implementation and verification of fundamental combinational circuits including Full Adders, Multiplexers, and Vector arithmetic using the Makerchip simulation environment.



