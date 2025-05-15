# FULL_ADDER_SUBTRACTOR

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

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

FULL ADDER

![Screenshot 2024-12-16 084637](https://github.com/user-attachments/assets/09dec625-e7ae-4818-b29f-2208de86d7cc)


FULL SUBRACTOR

![Screenshot 2024-12-16 084653](https://github.com/user-attachments/assets/c587b910-aca3-423c-8ddf-6393cdef48e7)


**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. 


Developed by:ANBUDURAI.A

RegisterNumber:212224230018


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

**RTL Schematic**

FULL ADDER 

![Screenshot 2024-12-16 084427](https://github.com/user-attachments/assets/0bd2c50f-d0e0-4016-9854-65cc8407666f)

FULL SUBRACTOR

![Screenshot 2024-12-16 084436](https://github.com/user-attachments/assets/569e4031-c072-441b-ac41-2c31a00f30cc)

**Output Timing Waveform**

FULL ADDER

![Screenshot 2024-12-16 084449](https://github.com/user-attachments/assets/468f5fa6-b921-4c6c-b0c9-82f53e683327)


FULL SUBRACTOR

![Screenshot 2024-12-16 090327](https://github.com/user-attachments/assets/f47d62ac-7558-4ab1-bd56-913210aac3bd)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



