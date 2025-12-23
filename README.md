# Building a 2 bit calculator

Computer science logic: representing throguh logic gates 

## Introducing half adder:
A half adder is a basic digital circuit that *adds two one bits* (Take X and Y), to produce a Sum (S) and a carry (C).

<p align="center">
  <img src="https://github.com/user-attachments/assets/3c5438eb-ba17-4389-8d1d-38d2d56be098" width="600">
</p>

To represent these with logic gates, we need to be introduced to the XOR and AND gate:

---

### XOR gate 

A XOR or Exclusive OR gate oupts a 0 if the input is the same, and 1 if the inputs are different. It acts as an **inequality detector**, or **anti-coincidence gate**. The boolean logic is

Q = A'B + AB'

XOR Gate truth table:
| (Bit 1 input) X  | (Bit 2 input) Y | (Output) Q |
| ------------- | ------------- | ------------- |
| 0  | 0 | 0  |
| 0  | 1  | 1 |
| 1  | 0  | 1  |
| 1  | 1  | 0  | 

*Constructed using AND, OR and NOT, (first row of the truth table below)*

<p align="center">
  <img src="https://github.com/user-attachments/assets/40e873ad-23ba-44e7-88d2-a92614d03cba" width="650">
</p>

---

### AND gate
An AND gate is a basic logic gate. You have two transistors in series with each other, both transistors gates would need to be on (1) to allow the flow to current to the output. 

The boolean logic is multiplying the two inputs to produce the value of:
Q = XY

<p align="center">
  <img src="https://github.com/user-attachments/assets/8ae73390-bfaa-460e-8a23-5219bc85c94f" width="650">
</p>

| (Bit 1 input) X | (Bit 2 input) Y | (Output) Q |
|-----------------|-----------------|------------|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

---

When you put the two logic gates together, you get the logic gate diagram of a half adder: 

<p align="center">
  <img src="https://github.com/user-attachments/assets/c5588795-6c19-496b-a73f-6b31c55a2806" width="600">
</p>

This makes the final truth table of a half adder to be:

| (Bit 1 input) X  | (Bit 2 input) Y | (Carry) C | (Sum) S |
| ------------- | ------------- | ------------- | ------------- |
| 0  | 0 | 0 | 0 |
| 0  | 1  | 0 | 1 |
| 1  | 0  | 0  | 1 |
| 1  | 1  | 1  | 0 |

and this works perfect as 1 + 1 =2, which is binary is 10, while 1+0 is just 1.  

## Introducing the Full Adder 
A full adder is able to add three 1 bit inputs to produce a sum and carry bit. But a full adder wont be possible without the carry bit of the past calculation. Without a carry bit, it wont be able to add the three numbers, making it relient on either another full adder or a half adder.

