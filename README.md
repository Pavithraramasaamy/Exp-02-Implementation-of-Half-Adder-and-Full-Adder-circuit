```
Developed by: Pavithra R
RegisterNumber: 212222230106
```
# Exp-03-Implementation of Half Adder and Full Adder circuit

# Implementation of Half Adder and Full Adder circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
```
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
# HALF ADDER:
module exp3(A,B,sum,carry);
input A,B;
output sum,carry;
assign sum= A^B;
assign carry = A&B;
endmodule

# FULL ADDER:
module ex3(A,B,Cin,sum,carry);
input A,B,Cin;
output sum,carry;
assign sum= A^B^Cin;
assign carry = (A&B)|((A^B)&Cin);
endmodule
*/
```
# Logic symbol 
![211153062-37e74d24-0b67-4d13-b795-0c759a3a22c9](https://github.com/Pavithraramasaamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118596964/cfc5468f-414e-4b58-b15a-ad3215b02c7f)

### RTL
HALF ADDER


![RTL ha](https://github.com/Pavithraramasaamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118596964/31ebfad5-bb7d-4b2e-984c-d23b4d11a642)


FULL ADDER

 ![RTL FULL](https://github.com/Pavithraramasaamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118596964/7e83b429-3d71-4a31-9389-6cf13617b3ac)

### TIMING DIAGRAM
HALF ADDER

![hawave](https://github.com/Pavithraramasaamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118596964/7c61d1be-85f3-403c-a5c5-e0a28faa71f7)


FULL ADDER

![ex3 full](https://github.com/Pavithraramasaamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118596964/dc8deeec-379d-4d14-8e2d-6f7e4a5446ae)

### TRUTH TABLE 


HALF ADDER


![211153259-99999f9f-7f34-45a8-a2cd-4aa1d1f216e1](https://github.com/Pavithraramasaamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118596964/966b41bc-32c1-45cf-b738-4aa0df5433b4)


FULL ADDER

![211153262-9733a71c-5534-4055-9fc7-88d63cc78463](https://github.com/Pavithraramasaamy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118596964/d27605ea-c643-4653-a794-378caa4167de)


### Result:
Thus the implementation of half adder and full adder circiut are stuided and the truth table
for different logic gates
