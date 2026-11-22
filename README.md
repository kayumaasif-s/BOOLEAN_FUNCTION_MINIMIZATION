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
~~~
module Exp2DE (
	input A,B,C,D,
	output F
);

assign F = (~A & ~B & ~C &~D) |
			  ( A & ~C & ~D)     |
			  (~B &  C & ~D)     |
			  (~A &  B &  C)     |
			  ( B & ~C &  D);
			  
endmodule
~~~

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: DEEPIKA.U RegisterNumber:212225040060*/

**Truth table**

<img width="483" height="292" alt="image" src="https://github.com/user-attachments/assets/23abf19b-7ebe-474a-a27f-02328e48215f" />

**RTL realization**

<img width="1920" height="1080" alt="Screenshot 2026-10-23 102720" src="https://github.com/user-attachments/assets/4ea82a67-2a02-462a-9911-032065feeeef" />

**Timing Diagram**

<img width="1920" height="1080" alt="Screenshot 2026-11-22 115504" src="https://github.com/user-attachments/assets/5a61bb70-f030-4a70-8872-617de92a6c90" />



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

