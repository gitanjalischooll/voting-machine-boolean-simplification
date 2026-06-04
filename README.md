# voting-machine-boolean-simplification
A Digital Logic Design project that implements a 3-input majority voting machine using Boolean Algebra and K-Map simplification. The system determines the winning output when two or more voters support the candidate.

A simple Digital Logic Design project that implements a **3-input Majority Voting Machine** using **Boolean Algebra** and **K-Map Simplification**.

## 📖 Overview

This project demonstrates how a combinational logic circuit can be used to determine the majority decision among three voters.

Each voter provides a binary input:
- **1** → Vote in favor
- **0** → Vote against

The candidate wins if **two or more voters vote in favor**.

This project highlights the practical application of Boolean Algebra and Logic Gates in designing digital systems.

---

## 🎯 Problem Statement

There are three voters: **A, B, and C**.

The output should satisfy the following conditions:

- **F = 1** → Candidate Wins (Majority Vote)
- **F = 0** → Candidate Loses

The output becomes HIGH only when at least two inputs are HIGH.

---

## 📊 Truth Table

| A | B | C | F |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 0 |
| 0 | 1 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 1 |

---

## 🧮 Boolean Expression

### Expression obtained from the Truth Table:

**F = A'BC + AB'C + ABC' + ABC**

### Simplified using Boolean Algebra / K-Map:

**F = AB + AC + BC**

This simplified expression minimizes the number of logic gates required, making the circuit more efficient.

---

## 🔌 Circuit Design

The circuit consists of:

- Three 2-input AND Gates
  - A · B
  - A · C
  - B · C

- One OR Gate to combine the outputs.

### Final Output Equation:

**F = AB + AC + BC**

An LED is connected to the output to indicate whether the candidate wins or loses.

---

## ⚙️ Working

1. Each switch acts as a voter input.
2. If two or more switches are turned ON, the output LED glows.
3. If fewer than two switches are ON, the LED remains OFF.

This demonstrates the working principle of a majority voting system using combinational logic.

---

## 🛠️ Components Used

### Hardware
- IC 7408 (AND Gate)
- IC 7432 (OR Gate)
- Breadboard
- 3 Toggle Switches
- LED
- 220Ω Resistor
- Connecting Wires
- 5V DC Power Supply

### Software (Optional)
- Logisim
- Proteus
- Tinkercad Circuits
- Multisim

---

## 🚀 Applications

- Electronic Voting Systems
- Decision Making Circuits
- Majority Detection Systems
- Fault Tolerant Digital Systems
- Digital Logic Laboratory Experiments

---

## 🔮 Future Scope

- Extend the design for N-number of voters.
- Implement using Microcontrollers or Arduino.
- Develop a complete Electronic Voting Machine (EVM).
- Integrate display and vote counting features.

---

## 📂 Project Files

- Project Presentation (.pptx)
- Circuit Diagram
- Working Model Images (Optional)
- README.md

---

## 📚 References

- M. Morris Mano – *Digital Logic and Computer Design*
- Logisim
- Tinkercad Circuits

---

## 👩‍💻 Developed By

**Gitanjali Jain (B243)**  

---

### ⭐ If you found this project useful, consider giving this repository a star!
