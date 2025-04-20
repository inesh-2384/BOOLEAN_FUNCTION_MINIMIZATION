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
Developed by: INESH n
RegisterNumber:212223220036

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
**RTL realization**
![image](https://github.com/inesh-2384/BOOLEAN_FUNCTION_MINIMIZATION/assets/146412203/2486b875-7dcf-480d-b54b-4fe0a69944f4)
**Truth Table**
![image](https://github.com/inesh-2384/BOOLEAN_FUNCTION_MINIMIZATION/assets/146412203/f5be67c0-fd64-41c1-90df-996bf33646df)

**Output:**

**RTL**
**Timing Diagram**
![image](https://github.com/inesh-2384/BOOLEAN_FUNCTION_MINIMIZATION/assets/146412203/260d04ef-1a25-4030-a284-f3231ef8ec4f)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

