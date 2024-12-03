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

module booleanfunction(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
assign x1= (~a)&(~b)&(~c)&(~d);
assign x2= (a)&(~c)&(~d);
assign x3= (~b)&(c)&(~d);
assign x4= (~a)&(b)&(c)&(d);
assign x5= (b)&(~c)&(d);
assign f1= x1|x2|x3|x4|x5;
assign x6= (x)&(~y)&(z);
assign x7= (~x)&(~y)&(z);
assign x8= (~w)&(x)&(y);
assign x9= (w)&(~x)&(y);
assign x10= (w)&(x)&(y);
assign f2= x6|x7|x8|x9|x10;
endmodule
REGISTER NUMBER:24900567
NAME:DHINESH


**RTL realization**

**Output:**

**RTL**
![Screenshot 2024-12-03 081015](https://github.com/user-attachments/assets/5549e472-b888-4c14-ae1d-144ef411a2bf)

**Timing Diagram**
![Screenshot 2024-12-03 081431](https://github.com/user-attachments/assets/ce1b9ed5-d3b5-4fc2-af04-9172e8ca074b)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

