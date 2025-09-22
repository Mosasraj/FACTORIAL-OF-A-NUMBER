# FACTORIAL-OF-A-NUMBER
# FACTORIAL OF A NUMBER USING 8051 (Keil)

## AIM
To write and execute an Assembly language program to perform the factorial of a number using 8051 Keil.

---

## APPARATUS REQUIRED
- Personal computer with Keil software

---

## ALGORITHM
1. **Start**
2. **Input**: Read the number `n`.
3. **Initialize**:
   - Set factorial to `1`.
   - Set `i` to `1`.
4. **Loop**: While `i` is less than or equal to `n`:
   - Multiply factorial by `i`.
   - Increment `i` by `1`.
5. **Output**: Store or print the value of factorial.
6. **End**

---

## FLOWCHART
<img width="506" height="525" alt="image" src="https://github.com/user-attachments/assets/f3b47187-6f0f-490c-8704-f2973cb2b276" />


---

## PROGRAM
```asm
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
OUTPUT
![WhatsApp Image 2025-09-22 at 19 33 44_3dd0de45](https://github.com/user-attachments/assets/c3001bf4-fa48-4dec-8082-483550bb5f13)

![WhatsApp Image 2025-09-22 at 19 35 18_378f6d89](https://github.com/user-attachments/assets/04750cd6-d291-4c24-86b7-15063f5e34e5)

---
<img width="421" height="521" alt="image" src="https://github.com/user-attachments/assets/1d3fefba-7e48-48ad-aa05-190d7814af73" />

---

RESULT

Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.

---


