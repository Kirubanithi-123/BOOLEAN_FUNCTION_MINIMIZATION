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
``
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
``

## Developed by:S.KIRUBANITHI
## RegisterNumber:212223220047


**RTL realization**
![Screenshot 2024-03-25 235246](https://github.com/Kirubanithi-123/BOOLEAN_FUNCTION_MINIMIZATION/assets/151388581/16218c9d-09ae-48ea-b1c8-70040af64698)


## Truth table
![Screenshot 2024-03-25 234731](https://github.com/Kirubanithi-123/BOOLEAN_FUNCTION_MINIMIZATION/assets/151388581/1f46e115-904e-4870-9a84-ad72c9643cf7)


**Timing Diagram**
![Screenshot 2024-03-25 234743](https://github.com/Kirubanithi-123/BOOLEAN_FUNCTION_MINIMIZATION/assets/151388581/56d6a1a1-04e8-4cac-a85d-b8689e5a7e4c)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

