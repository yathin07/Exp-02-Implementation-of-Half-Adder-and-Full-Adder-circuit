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

Developed by: YATHIN REDDY T
RegisterNumber: 23007417 

*/

##Code:

module full_adder(x, y, z, s, c, x1, x2, x3); 
input x, y,z; 
output s ,c, x1, x2, x3; 
xor(x1, x, y); 
xor(s, x1, z);
and(x2, x, y); 
and(x3, x1, z); 
or(c, x2, x3); 
endmodule

### Output:
### RTL:

Full Adder:

![image](https://github.com/yathin07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841679/9e0e0e32-07ff-42ca-b665-9b938221f9a8)

Half Adder:

![image](https://github.com/yathin07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841679/594be27d-a1f3-4b9c-a022-84fcc72b6508)


### TIMING DIAGRAM

Full Adder:

![image](https://github.com/yathin07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841679/55e4dbf3-2454-41fb-a496-d326b02d87b5)

Half Adder:

![image](https://github.com/yathin07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841679/471670b2-1141-4df9-921a-f166ea5a6b52)


### TRUTH TABLE 

Full Adder:

![image](https://github.com/yathin07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841679/177c1b30-ac2e-40f3-9494-b9bf32683de4)

Half Adder:

![image](https://github.com/yathin07/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/139841679/f2e6b757-e6fe-4c99-a367-952f9e33fcde)



### Result:

Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
