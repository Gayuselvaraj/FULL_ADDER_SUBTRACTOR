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

Full subractor:

![WhatsApp Image 2024-12-09 at 06 43 28_91139540](https://github.com/user-attachments/assets/a0523ea0-4539-40bd-8df2-77d01183d7e7)



**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

**RTL Schematic**
Full adder: 
![WhatsApp Image 2024-12-09 at 07 14 47_4ddaf5c1](https://github.com/user-attachments/assets/4ff53f94-4ac7-49b8-b3f7-06d9c011ff4a)

Full subractor:
![WhatsApp Image 2024-12-09 at 07 14 49_b0f2f9c1](https://github.com/user-attachments/assets/a05f28aa-2488-4731-b0bf-50d2d0301be1)


**Output Timing Waveform**
Full adder:
![WhatsApp Image 2024-12-09 at 07 14 45_9352da50](https://github.com/user-attachments/assets/9f248d42-2b22-4d16-b32f-1562f3fa36d6)

Full subractor:
![WhatsApp Image 2024-12-09 at 07 14 48_3b257d37](https://github.com/user-attachments/assets/dc618b0f-7752-4a80-b5ef-21e1fe0d80bc)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



