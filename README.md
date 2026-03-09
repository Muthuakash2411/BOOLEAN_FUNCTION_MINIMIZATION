# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime


**Truth Table**

<img width="805" height="442" alt="image" src="https://github.com/user-attachments/assets/9f12f19b-189f-4396-a87d-8d988c9ed600" />

<img width="797" height="421" alt="image" src="https://github.com/user-attachments/assets/5bff25cc-42bd-4589-ae44-d2d562f0ad63" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
````
Developed by:MUTHUAKASH M
RegisterNumber:212225230194

module exp2(w,x,y,z,a,b,c,d,f1,f2);
input w,x,y,z,a,b,c,d;
output f1,f2;
assign f1=(~a&~b&~c&~d)|(a&~c&~d)|(~b&c&~d)|(~a&b&c&d)|(b&~c&d);
assign f2=(x&~y&z)|(~x&~y&z)|(~w&x&y)|(w&~x&y)|(w&x&y);
endmodule

````
**RTL realization**
<img width="772" height="809" alt="image" src="https://github.com/user-attachments/assets/91cfb728-14c4-4f58-8f81-4388012e462f" />

**Timing Diagram**
<img width="1919" height="861" alt="image" src="https://github.com/user-attachments/assets/5b434f90-875e-450c-9b7b-7d30091c2446" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

