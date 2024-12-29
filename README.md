# FULL_ADDER_SUBTRACTOR
# DATE : 22/10/2024
Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**TRUTH TABLE**

![WhatsApp Image 2024-12-21 at 09 59 29_3fa8a637](https://github.com/user-attachments/assets/15ceea09-518d-4ba0-835c-1833067f5e5c)

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**TRUTH TABLE**

![WhatsApp Image 2024-12-21 at 09 59 48_8813293e](https://github.com/user-attachments/assets/16e3534c-1125-499b-bcce-a010cdbd32be)

**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
```
i)FULL ADDER

module fa(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^c);
assign carry= ( (a & b)| ( cin &(a ^ b ));
endmodule

ii)FULL SUBTRACTOR

module fs(a,b,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference= ( (a ^ b)^bin);
assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b )));
endmodule
```

Developed by:S HEMANTH KUMAR RegisterNumber:24011247*/

**RTL Schematic**
![Screenshot (25)](https://github.com/user-attachments/assets/f82ca736-d9cb-46eb-a97e-2281be6ef6ba)

![Screenshot (29)](https://github.com/user-attachments/assets/d40a0339-cfb3-4c79-9137-9cc682652100)

**Output Timing Waveform**
![Screenshot (26)](https://github.com/user-attachments/assets/91c2b8db-dfda-4332-96ab-eb2919c2d8fd)

![Screenshot (30)](https://github.com/user-attachments/assets/8f38dfc4-23bb-47ba-9385-86ca4415be9e)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



