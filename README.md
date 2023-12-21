## Name: Santhosh D M
## Reg.no:212223050044
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
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
HALF ADDER
```
module exphalf(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule

```
FULL ADDER
```
module expfull(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule
```
## Truth table
Half adder
![291242929-e917b3ac-1816-4978-908d-2ae7478dd918](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/0cfe64eb-fe0c-46fe-a7d6-79cb6fbb335a)
Full adder
![291243156-abedc1c1-49ab-4853-b02a-739e2553ba88](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/bf2e6ca5-be40-4e9b-865a-6d34b1cc0488)

### RTL viewer

HALF ADDER
![291243374-c07ee31d-47f9-465e-b556-63e83091da5e](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/a5f58928-0cdc-4342-b1d7-5fc7c3717bb5)

FULL ADDER
![291243508-c8fbda02-6596-4b69-92be-d2e23b879e4d](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/8e886da1-b810-4d31-85b3-ed004468fcd2)



### TIMING DIAGRAM
HALF ADDER
![291247827-f3342818-9d29-4b11-b6f4-e08152766f67](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/46e31458-91c8-451f-ab48-8a7de5087a96)

FULL ADDER
![291248032-ef0b46e5-ac8c-4449-be68-11884b873cc6](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/1dc63f37-7efe-47b2-8924-a94461f94bff)



### Result:
Thus the different digital IC's are studied and the truth table for different logic gates are verified.
