# Task 14: Karnaugh Maps and Logic Circuit – Burglar Alarm

## Objective
To design a simple burglar alarm using logic gates by analyzing door and key inputs with a Karnaugh Map (K-map).

---

## Inputs and Output
- **Door (D):**
  - 0 = Closed  
  - 1 = Open  
- **Key (K):**
  - 0 = OFF (Not pressed)  
  - 1 = ON (Pressed)  
- **Output (A):**
  - 0 = No Alarm  
  - 1 = Alarm (LED ON)

---

## Cases Considered
I analyzed the system based on the given conditions:

- **Case 1: Key ON (K = 1)**
  - Door open or closed → No alarm  

- **Case 2: Key OFF (K = 0)**
  - Door closed → No alarm  
  - Door open → Alarm ON  

---

## Truth Table (used ai to generate this table)

| K | D | A |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 0 |
| 1 | 1 | 0 |

---

## Karnaugh Map (used ai to generate this table)

| K\D | 0 | 1 |
|-----|---|---|
| 0   | 0 | 1 |
| 1   | 0 | 0 |

Simplified expression from K-map:

A = K' · D

---

## My Approach
I used:
- Two slide switches (Door and Key)
- IC 74HC00 (NAND gates)
- LED as alarm indicator

Steps I followed:
1. I wrote the truth table based on given cases.
2. I drew the K-map to simplify the logic.
3. I derived the expression: **A = K' · D**.
4. Since I used only NAND gates:
   - I inverted the key input using a NAND gate
   - I combined inputs using NAND logic to implement AND
5. I connected an LED to show the alarm output.

---

## Circuit Description
- Key input is inverted to get **K'**
- K' is combined with Door input
- Output is connected to LED
- LED acts as the alarm indicator

---

## Working
- If **key is ON**, alarm is always OFF  
- If **key is OFF**:
  - Door closed → No alarm  
  - Door open → LED glows (alarm ON)

---

## Result
I successfully implemented the burglar alarm circuit.  
The LED glows only when:
- Key = OFF  
- Door = OPEN  

---

## Conclusion
- K-map helped me simplify the logic easily  
- NAND gates were used to implement the circuit  
- The circuit works correctly as a basic burglar alarm  

---

https://github.com/user-attachments/assets/a79e8741-9bf8-4c03-9b42-da807c6c61c0
