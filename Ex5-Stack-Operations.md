# Ex5 Stack Operations
## DATE:
## AIM:
To write a C function to perform push and pop operation of the stack in the infix to postfix conversion.

## Algorithm
1. Initialize an empty stack.
2. To push an element: increment top and store the element at stack[top].
3. To pop an element: check if the stack is empty; if not, return stack[top] and decrement top.
4. Use the push operation to store operators when converting infix to postfix. 
5. Use the pop operation to remove and print operators based on precedence while converting infix to postfix.  

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: SWETHA S
RegisterNumber: 212222230155
*/
```
```
/*
#include<stdio.h>

char stack[100];
int top = -1;

void push(char x)
{
   //write your coding here
   top=top+1;
   stack[top]=x;
}

char pop()
{
   //write your coding here 
   if(top == -1)
    return -1;
   else
    return stack[top--];
}
*/
```
## Output:
<img width="369" height="222" alt="image" src="https://github.com/user-attachments/assets/4160a169-8ee9-44a4-b7ff-3b1fc19d7b89" />



## Result:
Thus the C program to perform push and pop operation of the stack in the infix to postfix conversion is implemented successfully.
