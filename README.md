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
Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
Developed by:MAHALAKSHMI.R
RegisterNumber: 212223230117
module bm(A,B,C,D,F1); 
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

![image](https://github.com/dhivyadharshini2006/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979490/031857ac-e7e9-419e-885d-0646c38fd6de)

**RTL**

![image](https://github.com/dhivyadharshini2006/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979490/5f843a33-bf33-4900-abf1-4bb164d148a4)

**Truth table**

![image](https://github.com/dhivyadharshini2006/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979490/a0c859e5-9a05-428f-90a2-629eb3f49d51)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

