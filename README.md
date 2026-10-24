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
 module ex2 (a,b,c,d,w,x,y,z,f1,f2);
 input a,b,c,d,w,x,y,z; output f1,f2;
 assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
 assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
 endmodule
~~~
**Truth Table**


<img width="483" height="292" alt="image" src="https://github.com/user-attachments/assets/23abf19b-7ebe-474a-a27f-02328e48215f" />


**RTL realization**


<img width="700" height="415" alt="image" src="https://github.com/user-attachments/assets/d1ad7d32-b3f8-49dd-a233-473585b0cfe0" />



**Timing Diagram**


<img width="703" height="413" alt="image" src="https://github.com/user-attachments/assets/75249ebd-a85e-49ae-b42c-1b70513b0503" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
