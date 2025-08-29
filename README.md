# 8-Bit-Odd-or-Even-Using-8085

## Aim:
To write an 8085 microprocessor program to check whether a given 8-bit number is odd or even.

## Apparatus Required:
•	Laptop with an internet connection

## Algorithm:
1.	Load the number from a specified memory location into register A.
2.	Perform an AND operation with 01H to check the least significant bit (LSB).
3.	If the result is 0, the number is even; otherwise, it is odd.
4.	Store the result in a specific memory location (odd or even flag).


## Program:
```
LDA 4200H
ANI 01H
JZ L1
MVI A, 01H
JMP L2
L1: MVI A, 02H
L2: STA 4300H
HLT
```

## Output:

<img width="1896" height="843" alt="image" src="https://github.com/user-attachments/assets/dbdf2283-fc6b-426d-b3e9-f1349f34e8e1" />


<img width="1887" height="846" alt="Screenshot 2025-08-29 162210" src="https://github.com/user-attachments/assets/a21bdd4d-c2d3-49ca-a2ea-0c08718b2099" />







## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

