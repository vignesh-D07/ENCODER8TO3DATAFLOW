### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/user-attachments/assets/e74050f9-3e4d-4279-a1bf-a99c75baeb4b)

Figure 1 Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/user-attachments/assets/a420b3d4-af6d-42ef-a8e5-6ab1a2735298)

Figure 02  Encoder 8 * 3

**Procedure**

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

**PROGRAM**

```
Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by: VIGNESH D
RegisterNumber: 212224050059
```
```
module exp5(din,a,b,c);
input [0:7] din;
output a,b,c;
assign a=(din[4]| din[5]| din[6]| din[7]);
assign b=(din[2]| din[3]| din[6]| din[7]);
assign c=(din[1]| din[3]| din[5]| din[7]);
endmodule
```

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![image](https://github.com/user-attachments/assets/5276f70a-c4b8-4d4e-9126-7ed18fd3bb66)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![image](https://github.com/user-attachments/assets/82031c91-7eb3-4c21-af84-026a4c792f8c)


**RESULTS**
Thus Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables is implemented and verified.





