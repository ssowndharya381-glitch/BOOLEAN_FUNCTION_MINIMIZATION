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
module funct1(a,b,c,d,f1);    
input a,b,c,d;    
output f1;      
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));     
endmodule    


module funct2(w,x,y,z,f2);    
input w,x,y,z;    
output f2;    
assign f2=((~y & z)|( w & y )|(x & y));     
endmodule    

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber: SOWNDHARYA S 25009992


**RTL realization**

**Output:**
**RTL**
<img width="1419" height="801" alt="Screenshot 2025-11-22 214047" src="https://github.com/user-attachments/assets/25bb0268-40c9-46a7-a120-1f42598ff893" />
<img width="1347" height="849" alt="Screenshot 2025-11-22 214113" src="https://github.com/user-attachments/assets/905223c2-7dd4-4bbf-b3fb-e91edbda8217" />



**Timing Diagram**
<img width="1736" height="865" alt="Screenshot 2025-11-22 214153" src="https://github.com/user-attachments/assets/e7b0825d-0596-4966-8d71-7d14c8e5ec37" />
<img width="1533" height="855" alt="Screenshot 2025-11-22 214302" src="https://github.com/user-attachments/assets/7b19793d-b316-43f5-bf1e-14ccf1a3e7a0" />



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

