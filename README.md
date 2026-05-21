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

i) Half Adder :

<img width="720" height="436" alt="516122508-0774b6ad-7882-4059-872b-85194504ac90" src="https://github.com/user-attachments/assets/4175a704-2eb7-461f-8dcb-ad44dd68492e" />


ii) Half Subtractor :

<img width="720" height="423" alt="516123133-25fdf851-82d3-435f-8bd9-a1d34bf1d29f" src="https://github.com/user-attachments/assets/0c22c40c-b6f2-4624-ae5e-f2c1542a38a6" />


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

i) Half Adder :

    module half_adder(a, b, sum, carry);
    input a, b;
    output sum, carry;

    assign sum   = a ^ b;   
    assign carry = a & b;   

    endmodule

ii) Half Subtractor :

    module half_subtractor(a, b, diff, borrow);
    input a, b;
    output diff, borrow;

    assign diff   = a ^ b;        
    assign borrow = (~a) & b;     

    endmodule


Developed by: Shahina A

RegisterNumber : 212225040396

**RTL Schematic**

i) Half Adder :

<img width="1280" height="720" alt="516124844-d907cc06-8970-4a64-93c3-ad17e6ae304e" src="https://github.com/user-attachments/assets/af401bdd-dba9-48d6-a214-0b3b2afcf2a7" />


ii) Half Subtractor :

<img width="1280" height="720" alt="516125147-7d91a9f9-8c95-41a6-af8b-6720a82bc08c" src="https://github.com/user-attachments/assets/c5842841-bc1c-4af7-8cd1-8116a0f0f283" />


**Output/TIMING Waveform**

i) Half Adder :

<img width="1280" height="720" alt="516125580-f8456eec-55fc-4638-9028-d7611b2672ec" src="https://github.com/user-attachments/assets/14c7a348-7293-4820-9f6a-a8d7bab4d09a" />


ii) Half Subtractor :

<img width="1280" height="720" alt="516125880-a7cb55de-3e08-4402-9539-06f0ea5507fd" src="https://github.com/user-attachments/assets/1adc5ec1-6eb1-42ba-a1ae-3b26e582434d" />


**Result:**

Thus, The half adder and half subtractor circuit are designed and verified its truth table using Quartus using Verilog programming.
