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

FUNCTION 1 K-MAP
![Screenshot 2024-12-08 205715](https://github.com/user-attachments/assets/3709bc02-e621-42a7-9847-7b96d40e32af) 

FUNCTION 2 K-MAP

![Screenshot 2024-12-08 205731](https://github.com/user-attachments/assets/c6379c99-908d-4fbe-8750-e78f90ffd536)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```

module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
FUNCTION1
![Screenshot 2024-12-08 210448](https://github.com/user-attachments/assets/3214c4b9-123a-487b-b5ce-c2ee79135640)

FUNCTION 2
![Screenshot 2024-12-08 210503](https://github.com/user-attachments/assets/48a52879-0661-4c1d-ba86-7ea784910ae6)

Developed by:latchaya priyan S

RegisterNumber:24900388


**RTL realization**

**Output:**

**RTL**

FUNCTION 1
![Screenshot 2024-12-08 210516](https://github.com/user-attachments/assets/42a57705-0176-468f-a113-b3f0ddeda457)

FUNCTION 2
![Screenshot 2024-12-08 210524](https://github.com/user-attachments/assets/0da9ff6f-a707-475e-8192-bf8a2527c762)


**Timing Diagram**

FUNCTION 1
![Screenshot 2024-12-08 210808](https://github.com/user-attachments/assets/81cf8f53-f048-45f5-996e-5b206e419097)

FUNCTION 2
![Screenshot 2024-12-08 210817](https://github.com/user-attachments/assets/1aa42ee0-9b2f-4809-8f4f-ce22af575c05)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

