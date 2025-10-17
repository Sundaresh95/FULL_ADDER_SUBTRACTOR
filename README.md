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

<img width="774" height="544" alt="image" src="https://github.com/user-attachments/assets/49df58a0-c5cb-4224-b1d9-cd4daecdb948" />


**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

<img width="825" height="566" alt="image" src="https://github.com/user-attachments/assets/1eca81aa-52cb-42c9-909f-ee9a05bdf0f8" />


Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**
<img width="429" height="395" alt="image" src="https://github.com/user-attachments/assets/a62745df-4943-45f9-b57b-46d777b1a355" />
<img width="438" height="393" alt="image" src="https://github.com/user-attachments/assets/5e6cec74-be2e-46fa-9c6b-2b5128fb47bf" />

**Procedure**

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

**Program:**

module JK(J,K,Qt,Y);

input J,K,Qt;

output Y;

assign Y = J & ~Qt | ~K & Qt;

endmodul

**RTL Schematic**
<img width="1177" height="744" alt="image" src="https://github.com/user-attachments/assets/3df96d52-8a61-4e77-9b8e-ffb2b7fcb366" />
<img width="1351" height="542" alt="image" src="https://github.com/user-attachments/assets/f3bf8d43-3396-4b6e-9333-017eb0503773" />

**Output Timing Waveform**
<img width="1920" height="1201" alt="image" src="https://github.com/user-attachments/assets/4b4372ce-088c-441a-b494-f40e58d377fd" />

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



