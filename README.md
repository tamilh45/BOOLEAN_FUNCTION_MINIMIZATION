# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber: 212223110058
*/
```
module exp2(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule
```
# OUTPUT

**RTL realization**

![435600216-83b00688-53ce-4b6f-947d-6d64ec0e1623](https://github.com/user-attachments/assets/0e78eee7-3bbe-467a-afd1-a378f4c327d8)

**Truth Diagram**
![382659424-afc3a642-9382-4700-8677-6e9486d40c60](https://github.com/user-attachments/assets/bed77dc7-4924-4c26-932d-4c32f358d108)

**Timing Diagram**
![435614197-9ba00dd0-639f-4975-acaf-842cc5424570](https://github.com/user-attachments/assets/6eb52d9f-bae0-4e1c-a3bc-c51723229db4)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

