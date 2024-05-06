# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE:                                                                           
### REGISTER NUMBER : 212221040127
### AIM: 
To write a logic program to design a circuit like half adder and half subtractor.
###  Algorithm:
1. Start the Program
2. Design a AND gate logic if both inputs are 1 then output is 1.
3. Design a OR gate logic if any one of input is 1 then output is 1.
4. Design a XOR gate logic if both inputs are different then output is 1.
5. Design a NOT gate logic if input is 0 then output is 1.
6. Design a half adder and half subtractor using the rules.
7. Test the logic.
8. Stop the program.

### Program:
  Half Adder:
  ```py
half_adder(A, B, Sum, Carry) :-
    xor(A, B, Sum),
    and(A, B, Carry).

xor(0, 0, 0).
xor(0, 1, 1).
xor(1, 0, 1).
xor(1, 1, 0).

and(0, 0, 0).
and(0, 1, 0).
and(1, 0, 0).
and(1, 1, 1).

```
  Half subtracter:
  ```py
half_sub(A, B, Dif, Brr) :-
    xor(A, B, Dif),
    not(A, X),
    and(X, B, Brr).

xor(0, 0, 0).
xor(0, 1, 1).
xor(1, 0, 1).
xor(1, 1, 0).

and(0, 0, 0).
and(0, 1, 0).
and(1, 0, 0).
and(1, 1, 1).

not(1, 0).
not(0, 1).

```










### Output:
![image](https://github.com/Vasanth1234567/AI_Lab_2023-24/assets/86919099/8f65ca8c-41cf-437f-8eba-03e8f02ea591)
<br/>
![image](https://github.com/Vasanth1234567/AI_Lab_2023-24/assets/86919099/b33e3eac-e0d6-4d70-9a44-15250a607f3f)




### Result:
Thus the truth table of circuit verified sucessfully.
