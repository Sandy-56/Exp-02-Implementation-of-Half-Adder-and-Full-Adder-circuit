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
### 
Program:
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
Developed by: Santhosh D M
RegisterNumber: 23013934
*/
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
HALF ADDER
![267689047-a7cc3d34-404f-43f5-9cbc-d9f5f5ba28e9](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/3756be55-2a82-430e-9c22-6d9eece9112a)
FULL ADDER
![267689278-7667c24f-a414-4e2b-840e-2ce0335dfbae](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/350f56e0-796d-487d-9a06-0735f15b4b06)


### TIMING DIAGRAM
HALF ADDER

![267689451-61076839-9c19-4192-a86a-d7233a325961](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/3898f06e-6f1c-4c3e-9073-98f23b809bbf)
FULL ADDER
![267689613-e5f0bbf9-9197-4bbf-a392-1e1dcad2f804](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/8b92bf6d-3a46-4382-a980-bd51388e45c4)

### TRUTH TABLE 
HALF ADDER
![267688455-b8abff6e-d197-4edd-9219-a69d9cb76aa8](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/d12eb37f-6bfd-4e44-a9d1-1dad50529194)
FULL ADDER
![267688520-7278c4df-a0ac-43c2-b0e0-75a0dffe843a](https://github.com/Sandy-56/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152118022/ecf55bf9-75d1-4f9c-a159-be1098dfd6df)

### Result:
Thus the different digital IC's are studied and the truth table for different logic gates are verified.
