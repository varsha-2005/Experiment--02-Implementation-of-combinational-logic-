# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce
one output.

Combinational logic gates are digital circuits that produce outputs based solely on the current inputs.
These gates are the building blocks for implementing digital systems and are used in a wide range of
applications, including arithmetic and logic operations, memory devices, and control circuits.

The two functions, F1 and F2, can be implemented using a combination of logic gates such as AND
gates, OR gates, and NOT gates.

 

## Logic Diagram

## Procedure

1.Use module projname(input,output) to start the Verilog programmming.
2.Assign inputs and outputs using the word input and output respectively.
3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.
4.Use each output(RTL Viewer and Timing Diagram) to represent F1 and F2.
5.End the verilog program using keyword endmodule

## Program:
```
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by:varsha.g
RegisterNumber:212222230166
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
module exp2f1(A,B,C,D,f1);
input A,B,C,D;
output f1;
assign f1=(~B&~D)|(A&B&~C)|(~A&B&D);
endmodule
F2=xy’z+x’y’z+w’xy+wx’y+wxy
module exp2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=(~y&z)|(x&y)|(w&y);
endmodule 
*/
```
## RTL realization
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

![image](https://user-images.githubusercontent.com/119288183/237037673-34007f04-c4b5-4d74-9c1b-8543700d9409.png)


F2=xy’z+x’y’z+w’xy+wx’y+wxy

![image](https://user-images.githubusercontent.com/119288183/237038524-5a63b31b-6ae1-4e0b-93a0-01103e7bc97f.png)


## Output 
## Timing Diagram
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

![image](https://user-images.githubusercontent.com/119288183/237038828-5ffdc7c8-c652-45e4-bdfb-6a6fc839d43b.png)


F2=xy’z+x’y’z+w’xy+wx’y+wxy

![image](https://user-images.githubusercontent.com/119288183/237042193-1308c9aa-8e44-45c7-bc06-09b821767c55.png)



## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
