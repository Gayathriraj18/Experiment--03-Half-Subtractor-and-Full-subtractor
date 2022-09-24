# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure

## Program:
/*
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: Gayathri A
RegisterNumber:  212221230028

### HALF ADDER:
module full(output D,B,input x,y,z);
assign D = x^y;
assign B = (~x&y);
endmodule

### FULL ADDER:
module full(output D,B,input x,y,z);
assign D = x^y^z;
assign B = (~x&(y^z)|(yz));
endmodule
*/

## Output:

### HALF ADDER:

## Truthtable

![half tt](https://user-images.githubusercontent.com/94154854/192110075-426c599e-31d0-4fad-88da-b01ddfe9692c.png)






##  RTL realization

![ha rtl](https://user-images.githubusercontent.com/94154854/192110088-df9bf1f5-052c-4d7f-b87a-bf451a376458.png)




## Timing diagram 

![half time](https://user-images.githubusercontent.com/94154854/192110081-2f752b48-0c6b-471f-b3cf-ca3317083a0d.png)


### FULL ADDER:

## Truthtable

![full tt](https://user-images.githubusercontent.com/94154854/192110101-dc2270b8-a937-4380-82e2-2f00a0285835.png)


##  RTL realization

![full rtl](https://user-images.githubusercontent.com/94154854/192110111-7ef1ea0c-0012-42f3-a869-373cfa9fa972.png)



## Timing diagram :

![full time](https://user-images.githubusercontent.com/94154854/192110117-a6b1f636-6b7d-4b69-a1cb-f7ba259c2d69.png)




## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
