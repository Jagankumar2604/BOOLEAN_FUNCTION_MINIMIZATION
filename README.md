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

Developed by:Jagan Kumar V
RegisterNumber:25012671/*
```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
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
**Logic symbol & Truthtable:**
<img width="805" height="442" alt="image" src="https://github.com/user-attachments/assets/3977c400-0f23-4c25-831f-a0f98aa0fd18" />
<
**RTL realization**
<img width="613" height="781" alt="image" src="https://github.com/user-attachments/assets/88d6b945-fca7-497f-a307-68c1e9a4aea4" />
<img width="613" height="781" alt="image" src="https://github.com/user-attachments/assets/6978502b-0250-49a7-a836-17405507b1fc" />


**Output:**
<img width="1041" height="532" alt="image" src="https://github.com/user-attachments/assets/ab0c2f84-1348-4675-ada1-960dc63c0c07" />

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.



Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

