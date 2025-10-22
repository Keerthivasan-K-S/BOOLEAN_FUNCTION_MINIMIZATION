# BOOLEAN_FUNCTION_MINIMIZATION

## AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

## Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime


## Logic Diagram
<img width="805" height="442" alt="image" src="https://github.com/user-attachments/assets/c066f5ba-0508-494e-9d76-2fa30199b0c5" />

## Procedure

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:

Developed by: Keerthivasan K S
RegisterNumber: 212224230120

```.py
module Exp_2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```


## Output:

## RTL
<img width="433" height="446" alt="image" src="https://github.com/user-attachments/assets/7700bdcd-5716-45b5-90b2-d5b3af23acf9" />

## Timing Diagram
<img width="1041" height="532" alt="image" src="https://github.com/user-attachments/assets/b7280afd-2f41-4ace-b088-928778da2579" />

## Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

