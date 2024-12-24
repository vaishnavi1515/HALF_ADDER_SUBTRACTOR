# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Half Adder

Sum = A’B+AB’ =A ⊕ B Carry = AB

module ha(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule

Half Subtractor

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

module hs(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule

Developed by:VAISHNAVI V
Register Number:24900560

**Truth table**
Half Adder

Sum = A’B+AB’ =A ⊕ B Carry = AB

![Screenshot (58)](https://github.com/user-attachments/assets/97c92a6f-6272-4af0-a838-6f2fc3af58ce)

Half Subtractor

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

![Screenshot (57)](https://github.com/user-attachments/assets/72f6cb8b-9814-4148-b870-8cd71a4d939e)

*RTL*

Half Adder

Sum = A’B+AB’ =A ⊕ B Carry = AB

![exp 3 H A](https://github.com/user-attachments/assets/d9b9510e-7408-4eab-a4b4-767098fc8d0a)

Half Subtractor

Diff = A’B+AB’ =A ⊕ B

Borrow = A’B

![exp 3 H S](https://github.com/user-attachments/assets/056de08e-dfb7-407a-a17c-2212957b91a9)

**Output**

Half Adder

Sum = A’B+AB’ =A ⊕ B Carry = AB

![exp 3 H A out](https://github.com/user-attachments/assets/3b95dbb4-c7f1-4b87-9428-ea0629902e7b)

Half Subtractor

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

![exp 3 H S out](https://github.com/user-attachments/assets/d50b3ec1-ca33-453f-893e-8596f67df217)

**Result:**
The half adder and half subtractor circuit was verified.

 
