# 8×8 Baugh–Wooley Multiplier – Design & Layout (Cadence Virtuoso)

## Overview
This project presents the **schematic design and physical layout** of an **8×8 signed Baugh–Wooley multiplier**
implemented using **Cadence Virtuoso**. The multiplier supports signed multiplication using
two’s complement representation and follows a regular array-based architecture suitable for
full-custom VLSI design.

The complete design flow—from basic logic gates to the final multiplier—was implemented,
laid out, and verified using **DRC and LVS checks**.

---

## Aim
To design the circuit and physical layout of an **8×8 Baugh–Wooley multiplier** using
Cadence Virtuoso and verify its correctness through **DRC and LVS**.

---

## Tools Used
- Cadence Virtuoso (Schematic & Layout)

> **Note:** Since Cadence Virtuoso was accessed on an academic server, raw design databases
cannot be shared.
## All relevant schematics, layouts, and verification results are documented
## using screenshots and reports in the above report pdf.

---

## Baugh–Wooley Multiplier
The **Baugh–Wooley algorithm** is used for efficient signed multiplication in two’s complement form.
It rearranges and complements partial products so that subtraction is avoided, allowing the use
of a regular array multiplier structure.

Key features:
- Handles signed operands using two’s complement
- Uses **white cells** for normal partial products
- Uses **gray cells** for complemented sign-related partial products
- Maintains a uniform and layout-friendly structure

This regularity makes the architecture well-suited for full-custom layout design.

---

## Design Hierarchy
The multiplier was built hierarchically starting from basic blocks:

- AND gate
- NAND gate
- XOR gate
- Mirror Full Adder
- White Cell
- Gray Cell
- White Cell with Half Adder
- Complete 8×8 Baugh–Wooley Multiplier

Each block was designed at schematic level and then converted into a corresponding layout.

---

## Layout Design
The layout was implemented using standard CMOS layers including diffusion, polysilicon, and metal.
Care was taken to ensure proper connectivity, compact area usage, and adherence to design rules.

### Layout Details
- Approximate layout dimensions: **325 µm × 685 µm**
- Total transistor count: **1882**
- Area utilized: **0.223 mm²**

---

## Verification

### DRC (Design Rule Check)
- Ensured compliance with all fabrication rules such as spacing, width, and enclosure
- **Result:** DRC clean (no errors)

### LVS (Layout Versus Schematic)
- Verified electrical equivalence between schematic and layout
- **Result:** LVS matched successfully

These checks confirm that the layout is manufacturable and functionally correct.

---

