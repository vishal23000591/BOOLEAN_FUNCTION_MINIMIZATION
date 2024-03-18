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

Developed by: Vishal S RegisterNumber: 212223110063*/
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

**RTL realization**
![exp_2](https://github.com/vishal23000591/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139719/71527db3-2ca6-4cb6-a727-c22867a1bdcc)

**Timetable**
![FAF](https://github.com/vishal23000591/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139719/c30c2243-570c-4596-8438-958aeca14159)
![faf1](https://github.com/vishal23000591/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139719/e5170c5d-1e6f-47bc-9bf9-1d3cb6cd08d9)

**Timing Diagram**
![Screenshot 2024-03-18 084929](https://github.com/vishal23000591/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139719/48682bc2-165e-4b07-8d96-2f89d93630a1)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

