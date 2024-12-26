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
Full adder:

![WhatsApp Image 2024-12-09 at 06 42 56_245deb09](https://github.com/user-attachments/assets/51d3e627-a6ee-4abb-b983-4005e12d580b)

Full subtractor:

![WhatsApp Image 2024-12-09 at 06 43 28_91139540](https://github.com/user-attachments/assets/a0523ea0-4539-40bd-8df2-77d01183d7e7)



**Procedure**


1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

Developed by: Gayathri S 

RegisterNumber: 24900444

```
module fa(a,b,cin,sum,carry):
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^cin);
assign carry= ( (a & b)| ( cin &(a ^ b )));
endmodule

module fs(a,b,bin,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference= ( (a ^ b)^bin);
assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b ))));
endmodule
```

**RTL Schematic**

Full adder: 

![WhatsApp Image 2024-12-09 at 07 14 47_4ddaf5c1](https://github.com/user-attachments/assets/4ff53f94-4ac7-49b8-b3f7-06d9c011ff4a)

Full subtractor:


![393247469-371eb82f-6369-48ee-9fa9-b6d2c9a94d7f](https://github.com/user-attachments/assets/2f0a1bea-507d-4481-b6cf-8a7a0cb751d5)

**Output Timing Waveform**

**Full adder**

![393247468-39cbdaa9-7e4f-4c93-b207-3c42cb800bdc](https://github.com/user-attachments/assets/abe6df4c-b4f0-4ab0-aed2-839f8d8cae29)


**Full subtractor**

![393247470-f213dcc6-ddc8-4d99-8da3-d0ea3751b715](https://github.com/user-attachments/assets/8d8b2367-a3d8-44fa-9a0c-43c6c0d75eb1)



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



