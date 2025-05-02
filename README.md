
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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Madhu shrie J

RegisterNumber: 212224100034
```
 module exp_2(A,B,C,D,F1);
 
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


**RTL realization**

![Screenshot (84)](https://github.com/user-attachments/assets/4f00b3d5-feac-4a63-a1af-66f873a2e47b)


**Output:**


![Screenshot 2025-04-24 124219](https://github.com/user-attachments/assets/0c245dab-2bdc-430c-bc75-2806b2c9a0c2)


**RTL**

**Timing Diagram**
![Screenshot (85)](https://github.com/user-attachments/assets/20a4fac0-d0c1-4553-89e9-7efa6077621e)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

