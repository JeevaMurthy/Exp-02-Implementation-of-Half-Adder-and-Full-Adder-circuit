# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
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
### Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:JEEVA K
RegisterNumber:23013748

1.Program to design a half adder:
module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule

1.Program to design a full adder:
module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
Logic symbol & Truthtable
```
### Output:
### RTL realization:
## HALF ADDER:
![image](https://github.com/JeevaMurthy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147222117/f228e5c3-0d6f-4a3f-9bff-c63f01550438)

## FULL ADDER:
![image](https://github.com/JeevaMurthy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147222117/82ae5413-6184-4f9c-833f-2af48d75259e)

### TIMING DIAGRAM:
## HALF ADDER:
![image](https://github.com/JeevaMurthy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147222117/913e9432-d376-4220-9cef-ac85e9ed9027)

## FULL ADDER:
![image](https://github.com/JeevaMurthy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147222117/798af4d4-b533-4d34-898c-5d2e8751b300)



### TRUTH TABLE:
## HALF ADDER:
![image](https://github.com/JeevaMurthy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147222117/9ea99d73-5f7e-49aa-bd86-28e93c28d33f)

## FULL ADDER:
![image](https://github.com/JeevaMurthy/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147222117/9b116a64-5ec0-4b0a-b17f-e5262e7dd885)



### Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
