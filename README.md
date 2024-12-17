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
module experiment2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module experiment2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:S Abinav Aaditya
Register number: 24002354


**RTL realization**
![Screenshot 2024-11-26 201156](https://github.com/user-attachments/assets/0b42be40-cd5b-49fe-b24c-b19b0e1e11f2)
![25](https://github.com/user-attachments/assets/b7a08d50-0655-43f4-a0ea-390c1f578473)

**Timing Diagram**
![Screenshot 2024-11-26 201511](https://github.com/user-attachments/assets/b0d309ff-5c4b-44d9-9723-5839488e3442)
![26](https://github.com/user-attachments/assets/274743d7-ae0f-4908-aafe-773edce6dce8)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

