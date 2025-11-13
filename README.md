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
module exp_2(A, B,C,D,W,X,Y,Z,F1,F2);
input A, B, C,D,W,X,Y,Z;
wire w1,w2,w3,w4,w5,w6,w7,w8,w9,w10;
output F1,F2;
assign w1=(~A)&(~B)&(~C)&(~D);
assign w2=(A)&(~C)&(~D);
assign w3=(~B)&(C)&(~D);
assign w4=(~A)&(B)&(C)&(D);
assign w5=(B)&(~C)&(D);
assign w6=(X)&(~Y)&(Z);
assign w7=(~X)&(~Y)&(Z);
assign w8=(~W)&(X)&(Y);
assign w9=(W)&(~X)&(Y);
assign w10=(W)&(X)&(Y);
assign F1=w1|w2|w3|w4|w5;
assign F2=w6|w7|w8|w9|w10;
endmodule
```


## Output:

## RTL
![WhatsApp Image 2025-11-13 at 14 11 38_0f6d681d](https://github.com/user-attachments/assets/34220cc6-5d6e-4ca1-a1c1-5b50494fa0b9)

## Timing Diagram
![WhatsApp Image 2025-11-13 at 14 12 00_9ad65bd2](https://github.com/user-attachments/assets/5f8602ab-97fc-4324-8f27-83522c6179ce)

## Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

