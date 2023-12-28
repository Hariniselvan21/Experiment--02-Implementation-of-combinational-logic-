# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime

## Theory
Logical gates are electronic circuits which perform logical functions on one or more inputs to produce one output 
 
## Logic Diagram

![image](https://github.com/Hariniselvan21/Experiment--02-Implementation-of-combinational-logic-/assets/155089072/23b89092-ab9f-4b54-9b93-4d99029ecc07)

## Procedure
Create a project with required entities. *Create a module along with respective file name. *Run the respective programs for the given boolean equations. *Run the module and get the respective RTL outputs. *Create university program(VWF) for getting timing diagram. *Give the respective inputs for timing diagram and obtain the results.

## Program:
/*Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: PRIYADHARSHINI S
RegisterNumber: 23003522
module combinational(a,b,c,d,w,x,y,z,fl,f2);
input a,b,c,d,w,x,y,z;
output fl,f2;
wire g1=((~a)&(~b)&(~c)&(~d)); 
wire g2=((a)&(~c)&(~d));
wire g3=((~b)&(c)&(~d));
wire g4=((~a)&(b)&(c)&(d)); 
wire g5=((b)&(~c)&(d));
assign fl=g1|g2|g3|g4|g5; 
wire g6=((x)&(~y)&(z));
wire g7=((~x)&(~y)&(z));
wire g8=((~w)&(x)&(y)); 
wire g9=((w)&(~x)&(y));
wire g10=((w)&(x)&(y)); 
assign f2=g6|g7|g8|g9|g10;
endmodule

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
### Developed by: Harini.N
### RegisterNumber: 212223050019 
*/
## RTL realization of NAND AND NOR gates

![image](https://github.com/Hariniselvan21/Experiment--02-Implementation-of-combinational-logic-/assets/155089072/f83631ce-a0ae-4af5-8d2c-93206cd9e94f)

 ## Truthtable of NAND gate:

 ![image](https://github.com/Hariniselvan21/Experiment--02-Implementation-of-combinational-logic-/assets/155089072/b9832c83-92e5-4e44-b9ed-c77d52698de9)

 ## Truthtable of NOR gate:
![image](https://github.com/Hariniselvan21/Experiment--02-Implementation-of-combinational-logic-/assets/155089072/3d525f6a-5ec9-4b98-9427-002ef5143deb)

## Timing Diagram
![image](https://github.com/Hariniselvan21/Experiment--02-Implementation-of-combinational-logic-/assets/155089072/e0c30db1-2ba6-4356-b1b8-17bd31d2f618)

## Result

Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
