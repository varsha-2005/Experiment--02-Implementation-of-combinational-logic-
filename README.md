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

https://user-images.githubusercontent.com/119218812/233413258-0ba8e708-35f4-4de6-8c66-601f8d7bd21f.png

F2=xy’z+x’y’z+w’xy+wx’y+wxy

https://user-images.githubusercontent.com/119218812/233413214-e3ccf259-0125-4113-a79c-487667e4dbe3.png

## Output 
## Timing Diagram
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

https://user-images.githubusercontent.com/119218812/233413642-d2ac08d2-d078-4945-bfd3-20521d3a6457.png

F2=xy’z+x’y’z+w’xy+wx’y+wxy

https://user-images.githubusercontent.com/119218812/233413570-6dd37770-b413-4752-ad60-e340214354b7.png
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
