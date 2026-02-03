# Makerchip IDE – Introduction and Lab Work

---

## Introduction

Let’s get started with Makerchip IDE.

Makerchip is a browser-based development environment used for digital design and hardware description using TL-Verilog. It allows users to design, simulate, and visualize hardware logic directly in the browser without requiring complex local tool installation.

The platform is widely used for learning modern hardware design methodologies, especially in RISC-V based processor design. It simplifies RTL development by introducing transaction-level abstraction and timing abstraction concepts.

Makerchip provides real-time simulation, waveform visualization, and debugging support, making it an efficient tool for both beginners and advanced hardware designers.

---

## Makerchip Platform Interface

Below is the Makerchip IDE workspace used for performing simulations and hardware design.

### Makerchip Workspace Screenshot

<img width="1799" height="942" alt="Screenshot 2026-02-03 155923" src="https://github.com/user-attachments/assets/aa586dd1-c5f1-4914-897a-f69fb7484fd2" />

---


## What is TL-Verilog?

TL-Verilog (Transaction Level Verilog) is an extension of traditional Verilog that simplifies hardware design by allowing designers to focus on logic behavior rather than low-level timing management.

Key features include:

- Automatic pipeline management  
- Timing abstraction  
- Reduced manual register handling  
- Improved code readability  
- Faster hardware prototyping  

---

## Why Makerchip is Used

Makerchip provides several advantages compared to traditional RTL simulation environments:

- Cloud-based IDE (No installation required)  
- Instant simulation feedback  
- Built-in visualization tools  
- Easy debugging support  
- Supports TL-Verilog coding  
- Ideal platform for RISC-V processor learning  

---

## Understanding Makerchip Workspace

The Makerchip interface mainly consists of:

### Code Editor

Used for writing TL-Verilog design and simulation code.
![editor](https://github.com/user-attachments/assets/e874884a-c72b-4cc6-99f9-89628609be1a)

### Output Window
Displays simulation results and debug messages.

### Waveform Viewer
Shows graphical representation of signal changes.
![wavefrom](https://github.com/user-attachments/assets/ed8f5d98-81f6-4cef-90d2-69482f1bfce5)

### Diagram View
![diagram](https://github.com/user-attachments/assets/7461989c-a76b-47ec-8ec5-e1e9bfd75b78)

Provides pipeline visualization and design flow understanding.

---

# Laboratory Experiments / Examples Performed

<img width="1397" height="768" alt="Screenshot 2026-02-03 152941" src="https://github.com/user-attachments/assets/0256bd1b-b0d0-4322-b351-30769f5a5dd5" />

---
## Lab 1: Combinational Logic – Basic Gate Implementation

---

### Objective

To design and simulate fundamental combinational logic gates using TL-Verilog in Makerchip IDE and analyze their behavior through waveform visualization.
---

## Introduction to Combinational Logic

Combinational logic circuits generate outputs based solely on present input values. These circuits do not contain memory elements and do not depend on clock signals.

In this lab, basic logic gates were implemented using TL-Verilog to understand their functionality and simulation behavior in Makerchip.

---
### 1. AND Gate
Logic: The output is 1 (high) only if both inputs are 1.

TLV Code: $out = $in1 && $in2;

Operator: The && symbol represents the Boolean AND operator.

<img width="1917" height="978" alt="and" src="https://github.com/user-attachments/assets/d4201aee-5006-4f07-9b7b-da8d7b068e79" />
---

### 2. Inverter 
Logic: Reverses the input signal. If the input is 1, the output is 0, and vice versa.

TLV Code: $out = ! $in1;

Operator: The ! symbol represents the Boolean NOT operator.

<img width="1896" height="918" alt="inverter" src="https://github.com/user-attachments/assets/c178a940-c3e0-4311-9da6-e44c1e094bf8" />
---
### 3. OR Gate
Logic: The output is 1 if at least one of the inputs is 1.

TLV Code: $out = $in1 || $in2;

Operator: The || symbol represents the Boolean OR operator.

<img width="1919" height="1003" alt="or" src="https://github.com/user-attachments/assets/3e5a2819-eb48-4c7f-98fa-7dcc021dab24" />
---
### 4. XOR Gate
Logic: The output is 1 if the inputs are different (one is 1, the other is 0).

TLV Code: $out = $in1 ^ $in2;

Operator: The ^ symbol represents the Boolean XOR operator.

<img width="1910" height="978" alt="xor" src="https://github.com/user-attachments/assets/89a830ba-e30c-4bd2-b12e-7989bef02e13" />
---

Description:
The screenshot above shows the Makerchip IDE navigation menu. The “Examples” option is highlighted in red to indicate where users can access predefined Verilog/TL-Verilog example projects. This section is useful for exploring sample designs, learning syntax, and understanding how different components work in the Makerchip environment. Selecting Examples opens a list of ready-to-run projects that can be used for hands-on practice and experimentation.










