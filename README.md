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
![Screenshot 2024-11-16 190105](https://github.com/user-attachments/assets/a1b4f98b-9def-4673-8587-280cf08c1895)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
module function1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Akash Prakash
RegisterNumber:24008757
![Screenshot 2024-11-16 185736](https://github.com/user-attachments/assets/89c67e79-a3a3-485a-82ef-d29112570ce7)


**RTL realization**
![Screenshot 2024-11-16 190000](https://github.com/user-attachments/assets/de141f2a-ef5d-4f73-a0d8-2199bbaf67a9)

**Output:**

**RTL**

**Timing Diagram**
a	b	c	d	~b	~d	~a	~c	(~b & ~d)	(~a & b & d)	(a & b & ~c)	f1 (final result)
0	0	0	0	1	1	1	1	1	0	0	1
0	0	0	1	1	0	1	1	0	0	0	0
0	0	1	0	1	1	1	0	1	0	0	1
0	0	1	1	1	0	1	0	0	0	0	0
0	1	0	0	0	1	1	1	0	0	1	1
0	1	0	1	0	0	1	1	0	1	0	1
0	1	1	0	0	1	1	0	0	0	0	0
0	1	1	1	0	0	1	0	0	1	0	1
1	0	0	0	1	1	0	1	1	0	0	1
1	0	0	1	1	0	0	1	0	0	0	0
1	0	1	0	1	1	0	0	1	0	0	1
1	0	1	1	1	0	0	0	0	0	0	0
1	1	0	0	0	1	0	1	0	1	1	1
1	1	0	1	0	0	0	1	0	1	0	1
1	1	1	0	0	1	0	0	0	0	0	0
1	1	1	1	0	0	0	0	0	1	0	1
![image](https://github.com/user-attachments/assets/d5d0dc83-4df9-470c-942b-e536cbe695f5)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

