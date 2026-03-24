# Factorial-of-Number-using-8051-
# FACTORIAL OF A NUMBER USING 8051 (Keil)
# AIM
To write and execute an Assembly Language Program to perform the factorial of a number using 8051 Keil.

# APPARATUS REQUIRED
Personal computer with Keil software
# ALGORITHM
1.Start
2.Input: Read the number n.
3.Initialize:
    *Set factorial to 1.
    *Set i to 1.
4.Loop: While i is less than or equal to n:
        *Multiply factorial by i.
        *Increment i by 1.
5.Output: Store or print the value of factorial.
6.End

# FLOWCHART
![WhatsApp Image 2026-03-24 at 11 30 22 AM](https://github.com/user-attachments/assets/c28de8fd-7545-49a4-88b7-86ed094f3230)
# PROGRAM
```
ORG 0000H
MOV DPTR,#4500H
MOVX A,@DPTR
MOV R0,A
INC DPTR
ACALL FACTORIAL
MOVX @DPTR,A
SJMP THIN
FACTORIAL:DEC R0
CJNE R0,#01H,PRODUCT
SJMP THICK
PRODUCT:MOV B,R0
MUL AB
ACALL FACTORIAL
THICK: RET
THIN:RET
END
```
# OUTPUT
![WhatsApp Image 2026-03-24 at 11 31 03 AM](https://github.com/user-attachments/assets/90ecb2eb-fc69-4433-8225-f561ea41d8ff)
# MANUAL CALCULATION
![WhatsApp Image 2026-03-24 at 11 31 37 AM](https://github.com/user-attachments/assets/f2636629-05a0-492e-a1bd-3bc55d8ccc74)
# RESULT
Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.


