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
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: MOHAMMAD FAIZAL SK
RegisterNumber:212223240092

module combinationalcircuit(A,B,C,D,F1);
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

**Output:**

**RTL realization**
![Screenshot 2024-03-24 141634](https://github.com/MOHAMEDRIDWAN/BOOLEAN_FUNCTION_MINIMIZATION/assets/146993368/62ea4916-36fc-4e78-b4b0-90848ff33935)

**Timing Diagram**
![Screenshot 2024-03-24 142440](https://github.com/MOHAMEDRIDWAN/BOOLEAN_FUNCTION_MINIMIZATION/assets/146993368/a1dfc5c5-20ae-457a-b244-ff068731e791)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

