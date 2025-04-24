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
```
Developed by:DHARSHINI R
 Register Number:212224220023
```
TRUTH TABLE:
![2 1](https://github.com/user-attachments/assets/00aacf21-40d2-4d42-bed6-dea13cfd0239)

![2 2](https://github.com/user-attachments/assets/6cbef969-9966-4364-b2c7-386096f9e33c)



**RTL realization**
![2 o](https://github.com/user-attachments/assets/6defb27a-72af-46fa-a89c-9c028ece91d5)

**Output:**
![2 ro](https://github.com/user-attachments/assets/cb340976-5ae1-445f-b25f-6a7613565057)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

