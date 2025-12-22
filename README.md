# Building a 2 bit calculator

Computer science logic: representing throguh logic gates 

## Introducing half adder:
A half adder is a basic digital circuit that *adds two one bits* (Take X and Y), to produce a Sum (S) and a carry (C).

<img width="984" height="311" alt="image" src="https://github.com/user-attachments/assets/3c5438eb-ba17-4389-8d1d-38d2d56be098" />

To represent these with logic gates, we need to be introduced to the XOR and AND gate:

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
<img width="1459" height="407" alt="image" src="https://github.com/user-attachments/assets/40e873ad-23ba-44e7-88d2-a92614d03cba" />

### AND gate
An AND gate is a basic logic gate. You have two transistors in series with each other, both transistors gates would need to be on (1) to allow the flow to current to the output. 

The boolean logic is multiplying the two inputs to produce the value of:
Q = XY

<img width="1568" height="665" alt="image" src="https://github.com/user-attachments/assets/8ae73390-bfaa-460e-8a23-5219bc85c94f" />

| (Bit 1 input) X  | (Bit 2 input) Y | (Output) Q |
| ------------- | ------------- | ------------- |
| 0  | 0 | 0 |
| 0  | 1  | 0 |
| 1  | 0  | 0  |
| 1  | 1  | 1  | 

When you put the two logic gates together, you get the logic gate diagram of a half adder: 
<img width="892" height="522" alt="image" src="https://github.com/user-attachments/assets/c5588795-6c19-496b-a73f-6b31c55a2806" />



