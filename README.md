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

**Truthtable**

![WhatsApp Image 2024-12-03 at 20 32 29_de8ca8bb](https://github.com/user-attachments/assets/a6ea4769-7016-4222-bc04-8c2826277d5f)

![WhatsApp Image 2024-12-03 at 20 32 29_bbe21538](https://github.com/user-attachments/assets/891ee06f-a563-401c-be43-839e9d6d6522)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Half Adder
     
     module ha(a,b,sum,carry);
     input a,b;
     output sum,carry;
     assign sum= (a ^ b);
     assign carry= ( a & b);
     endmodule

Half Subractor


    module hs(a,b,difference,borrow);
    input a,b;
    output difference,borrow;
    assign difference= (a ^ b);
    assign borrow= ( ~a & b);
    endmodule



Developed by: S.Ravant Vignesh

RegisterNumber:24900151  */

**RTL Schematic**
![WhatsApp Image 2024-12-03 at 20 32 28_4588eefe](https://github.com/user-attachments/assets/c4b05f1f-d223-4a34-802d-78e6aa328d88)

![WhatsApp Image 2024-12-03 at 20 32 29_6cc93646](https://github.com/user-attachments/assets/911cc235-6fc9-47e8-8953-bc801e80c926)

**Output/TIMING Waveform**
![WhatsApp Image 2024-12-03 at 20 32 30_c50f1ddd](https://github.com/user-attachments/assets/550c7aff-0bda-4984-8452-4a0c322a4982)

![WhatsApp Image 2024-12-03 at 20 32 30_e7bd3f37](https://github.com/user-attachments/assets/28c660b3-6744-4a52-a97f-360704b4671f)

**Result:**
Thus a half adder and half subtractor circuit is designed and verified its truth table inQuartus using Verilog programming.
