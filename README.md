# FACTORIAL-OF-A-NUMBER-USING-8051-KEIL

**AIM:**

To write and execute Assembly language Program to perform factorial of a number using 8051 keil.
APPARATUS REQUIRED: Personal computer with Keil software

**ALGORITHM:**

• Start  

• Input: Read the number n.  

• Initialize:  

•Set factorial to 1.  

•Set i to 1.  

• Loop: While i is less than or equal to n:  

•Multiply factorial by i.  

•Increment i by 1.  

• Output: Store or print the value of factorial.  

• End

**FLOW CHART:**
<img width="261" height="308" alt="image" src="https://github.com/user-attachments/assets/bffe89f6-3ba9-4294-b817-8b545f680e66" />

**Program:**

ORG 0000H   

MOV A,#04H  

MOV R0,A  

ACALL FACTORIAL  

MOV 40H,A  

SJMP THIN  

FACTORIAL:DEC R0  

CJNE R0,#01H,PRODUCT  

SJMP THICK   

PRODUCT:MOV B,R0  

MUL AB  

ACALL FACTORIAL  

THICK: RET  

THIN:  

END

**Output:**  

<img width="1891" height="982" alt="Screenshot 2025-11-11 213641" src="https://github.com/user-attachments/assets/84e33e0d-f77b-4e8f-83b1-2aa3462ea20f" />


**Manual Calculations:**  

<img width="450" height="700" alt="Screenshot 2025-11-11 230129" src="https://github.com/user-attachments/assets/fc609fec-8d6e-4372-a1b8-7ea8aa8ee412" />



**Result:**

Thus the factorial of a number using 8051 keil was calculated and shown the output.
