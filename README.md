## Name: Santhosh D M
## Register No: 212223050044
# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime

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
Switch ON the main switch if the output is 1, then the led glows.
If the output is 1, then the led glows.


### Program:
/*
## Half Adder
```
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule
```
## Full Adder
```
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule
```
## Truth Table
Half adder
![291242929-e917b3ac-1816-4978-908d-2ae7478dd918](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/26ddb90d-d13b-4bd6-926c-2f1ad815eb8e)
Full Adder
![291243156-abedc1c1-49ab-4853-b02a-739e2553ba88](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/28413e8c-9f8e-414b-b573-0f2ed5509f02)

### RTL Viewer
HalF adder
![291243374-c07ee31d-47f9-465e-b556-63e83091da5e](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/73efbeb6-aee5-4e28-a687-83b3516be23a)
Full Adder
![291243508-c8fbda02-6596-4b69-92be-d2e23b879e4d](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/702904b3-4058-4f97-82be-23b78fad47c5)


### TIMING DIAGRAM:
Half Adder
![291247827-f3342818-9d29-4b11-b6f4-e08152766f67](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/7c5ebb11-5936-4f7c-bcf2-c66c8c991688)




### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
