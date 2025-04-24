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

```/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Saikripa SK 
RegisterNumber:*/212224040284

module
sample2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~a)&(~b)&(~c)&(~d))|(a&
(~c)&(~d))|(~b)&c&(~d)|((~a)&b&c&d)|
(b&(~c)&d);
assign f2=(x&(~y)&z)|((~x)&(~y)&z)|
((~w)&x&y)|(w&x&(~y))|(w&x&y);
endmodule
```
**Logic symbol and truth table**

![image](https://github.com/user-attachments/assets/312a5b5e-6e0e-45ed-a690-10b9cc01ab4e)
![image](https://github.com/user-attachments/assets/02a84a58-7138-4cd2-a9a5-1c5e5ebed9f0)

**RTL realization**

![image](https://github.com/user-attachments/assets/5e3d61f0-59f4-4728-9f14-09d7d2e4d198)

**RTL Waveform**

![image](https://github.com/user-attachments/assets/28cdf32f-f657-4948-b2b4-212d541a332f)

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

