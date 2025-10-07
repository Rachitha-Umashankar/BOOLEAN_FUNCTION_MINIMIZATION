# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus II**

**Theory**

 Boolean function minimization is the process of simplifying Boolean algebraic
 expressions to reduce the number of logic gates and complexity in a digital circuit,
 leading to more efficient, faster, and less costly hardware
 For minimizing Boolean expressions,we can use a set of rules and laws (like distributive,
 associative, and complement laws) to simplify Boolean expressions. This method
 focuses on applying algebraic manipulations to reduce the complexity of the expression
 by eliminating redundant terms.
 
 Identity Law A ⋅ 1 = A, A + 0 = A
 
 Null Law A ⋅ 0 = 0, A + 1 =1

 Idempotent Law A ⋅ A = A, A + A = A
 
 Complement Law A ⋅ A′ = 0, A + A' = 1
 
 Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C
 
 De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′
 
 Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A
 
 Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C
 
 Commutative law A B = B A,A + B = B + A
 
**Logic Diagram**

![WhatsApp](https://github.com/user-attachments/assets/1fe31655-d601-453e-bc62-31d6c64f0f8b)

![What](https://github.com/user-attachments/assets/771ce9e7-14de-42a1-a603-c62605dc9709)

![hat](https://github.com/user-attachments/assets/c08512db-134e-4123-bc11-4cb97d63e964)

![Image](https://github.com/user-attachments/assets/a5ea59b8-b94c-4003-aad5-004ab0677736)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

i)
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

**RTL realization**

**Output:**

i)

![image](https://github.com/user-attachments/assets/a664db9b-15e4-48d5-9c6b-4e665c2b5094)

ii)

![im](https://github.com/user-attachments/assets/1f718bab-a533-4b50-9a07-c96f12de06f2)

**RTL**

**Timing Diagram**

i)

![image](https://github.com/user-attachments/assets/76d33072-3e83-4baf-9352-b60706b8f448)

ii)

![image](https://github.com/user-attachments/assets/90b73123-7fd6-4cc4-af39-87d82933eca7)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

