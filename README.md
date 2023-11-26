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
Developed by:PRIYADHARSHINI S
RegisterNumber:23003522

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
```
## Output:
## RTL realization:
## HALF ADDER:
![image](https://github.com/priyadharshini225/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138849213/a58d391c-14c0-48b2-9a37-93acdd089d9f)


## FULL ADDER:
![image](https://github.com/priyadharshini225/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138849213/7f3d4874-bc2a-43e0-b720-5dec31aa2e21)


## TIMING DIAGRAM:
## HALF ADDER:
![image](https://github.com/priyadharshini225/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138849213/711319a2-94c2-4f0f-b4bc-7b64b8dfca74)


## FULL ADDER:
![image](https://github.com/priyadharshini225/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138849213/11f7cf3b-6bb8-4f4a-805b-a551f2048a31)


## TRUTH TABLE:
## HALF ADDER:
![image](https://github.com/priyadharshini225/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138849213/e8da5a40-5107-455f-8183-2a1d34472be0)


## FULL ADDER:
![image](https://github.com/priyadharshini225/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/138849213/0a7bae15-fe63-4611-86c6-8d15a9e172ff)


## Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.




