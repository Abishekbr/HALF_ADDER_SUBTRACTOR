![Screenshot 2025-04-30 091318](https://github.com/user-attachments/assets/adf903f6-9f2b-4cc5-acbe-be1bf189c953)# HALF_ADDER_SUBTRACTOR

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

**Truthtable**
HALF ADDER
![Screenshot 2025-04-30 090333](https://github.com/user-attachments/assets/d275b078-e935-477e-b6cf-439371ba15e1)
HALF SUBTRACTOR
![Screenshot 2025-04-30 090348](https://github.com/user-attachments/assets/416b1651-cd45-4914-a3c6-9a6443e8686e)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
 Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:sai likitha RegisterNumber:24009865
module exp003(a,b,sum,cout,diff,borr);
input a,b;
output sum,cout,diff,borr;
xor g1(sum,a,b);
and g2(cout,a,b);
wire w1;
xor g3(diff,a,b);
not g4(w1,a);
and g5(borr,w1,b);
endmodule 

```

Developed by: RegisterNumber : 212224110002 / B.R.Abishek


**RTL Schematic**
![Screenshot 2025-04-30 090931](https://github.com/user-attachments/assets/38d371f3-92bc-4f08-a62e-29f9225e5276)
![Screenshot 2025-04-30 091318](https://github.com/user-attachments/assets/5a3ad4b6-2e9d-4a66-98c4-51ed25bebc2a)


**Output/TIMING Waveform**

**Result:**
 Thus the given half adder and subtractor is studied and verified in quartus using verilog program.
