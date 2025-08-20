# Ex4 Evaluation of prefix expression
## DATE:
## AIM:
To write a C function to evaluate the given prefix expression using stack and print the output of the given prefix expression from the stack inside the function . 

## Algorithm
1. Initialize an empty stack.
2. Read the prefix expression from right to left.
3. If the scanned character is an operand, push it onto the stack.
4. If the scanned character is an operator, pop two operands from the stack, apply the operator, and push the result back onto the stack. 
5. Repeat until the entire expression is scanned.
6. The final value remaining in the stack is the result of the prefix expression.  

## Program:
```
/*
Program to evaluate the given prefix expression
Developed by: SWETHA S
RegisterNumber:  212222230155
*/
```
```
/*
#include<stdio.h>
#include<string.h>
#include<ctype.h>

int s[50];
int top=0;

void push(int ch)
{
	top++;
	s[top]=ch;
}

int pop()
{
	int ch;
	ch=s[top];
	top=top-1;
	return(ch);
}

void evalprefix(char p[50])
{
    //Write your code here 
    int a,b,c,i;
    for(i=strlen(p)-1;i>=0;i--)
    {
        if(p[i] == '+')
        {
            a = pop();
            b = pop();
            c = a + b;
            push(c);
        }
        else if(p[i] == '/')
        {
            a = pop();
            b = pop();
            c = a / b;
            push(c);
        }
        else
        {
            push(p[i] - 48);
        }
    }
    printf("%d",pop());
}
*/
```
## Output:
<img width="329" height="217" alt="image" src="https://github.com/user-attachments/assets/9af16afd-2cb2-4da6-9cf6-39bb9727fe5b" />



## Result:
Thus, the C program to evaluate the prefix expression using stack and print the output of the given prefix expression from the stack inside the function is implemented successfully.
