# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher Software – Quartus prime

**Theory**
A combinational circuit is a circuit in which the output depends on the presentcombination of inputs. Combinational circuits are made up of logic gates. The output ofeach logic gate is determined by its logic function. Combinational circuits can be madeusing various logic gates, such as AND gates, OR gates, and NOT gates.


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

```
 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Eesha Ranka
RegisterNumber: 212224240040
```

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


![image](https://github.com/user-attachments/assets/2b1209a5-8d0e-452a-af3e-62902fa1ee58)


**Truth Table**

![image](https://github.com/user-attachments/assets/97ed0d9f-cb44-4ba6-ab38-4f647dbfe143)


**Timing Diagram**

![image](https://github.com/user-attachments/assets/1640cb4a-eae8-4cf4-92a5-65dec09718b5)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

