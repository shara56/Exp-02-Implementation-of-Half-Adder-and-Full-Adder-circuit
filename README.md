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
# Program:
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: SHARANGINI T K

RegisterNumber:  212222230143
```
Half adder program:
module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```

### Output:

HALF-ADDER:-

![image](https://user-images.githubusercontent.com/113497104/229346522-2f1ef177-709f-419a-9b41-f845ce48278a.png)

FULL-ADDER:-

![image](https://user-images.githubusercontent.com/113497104/229346974-f3d2fc44-ad78-4394-94d5-f11a6feec58d.png)

# RTL
HALF-ADDER:-

![image](https://user-images.githubusercontent.com/113497104/229346690-cb65b1cd-d0ec-41fe-9e3e-6db8a8119678.png)

FULL-ADDER:-

![image](https://user-images.githubusercontent.com/113497104/229346725-a1905c82-f5af-468e-a8dd-688080972588.png)

# TIMING DIAGRAM:
HALF-ADDER:-

![image](https://user-images.githubusercontent.com/113497104/229346774-66c12b94-ff2f-427d-903f-e3e0a9f2000a.png)

FULL-ADDER:-

![image](https://user-images.githubusercontent.com/113497104/229346817-d5f90ccc-00fb-4c95-9260-a03859eda548.png)

# TRUTH TABLE:
HALF-ADDER:-

![image](https://user-images.githubusercontent.com/113497104/229346884-35e719e0-28b2-4098-b3e5-e3f05cf6a0f6.png)

FULL-ADDER:-

![image](https://user-images.githubusercontent.com/113497104/229346922-29f46bd8-207d-47ec-a3b0-4ab55e6259bf.png)

# Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.










