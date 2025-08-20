# Ex2 Conversion of the infix expression into postfix expression
## DATE:
## AIM:
To write a C program to convert the infix expression into postfix form using stack by following the operator precedence and associative rule.

## Algorithm
1. Initialize an empty stack for operators and an empty output for the postfix expression.
2. Read the infix expression from left to right.
3. If the scanned character is an operand, add it to the postfix expression.
4. If the scanned character is (, push it onto the stack.
5. If the scanned character is ), pop and print all operators until ( is encountered.
6. If the scanned character is an operator, pop and print operators from the stack while they have higher or equal precedence, then push the scanned operator onto the stack.
7. After the entire expression is scanned, pop and print all remaining operators in the stack. 

## Program:
```
/*
Program to convert the infix expression into postfix expression
Developed by: SWETHA S
RegisterNumber:  212222230155
*/
```
```
/*
char IntoPost(char *exp)
{
    //write your code here
    char *e,x;
    e=exp;
    
    while(*e != '\0')
    {
        if(isalnum(*e))
        {
            printf("%c",*e);
        }
        else if(*e == '(')
        {
            push(*e);
        }
        else if(*e == ')')
        {
            while((x=pop()) != '(')
            {
                printf("%c" ,x);
            }
        }
        else
        {
            while(priority(stack[top]) >= priority(*e))
                printf("%c",pop());
            push(*e);    
            
        }
        e++;
    }
    while(top != -1)
    {
        printf("%c",pop());
    }
    
 return 1;   
}
*/
```
## Output:
<img width="446" height="145" alt="image" src="https://github.com/user-attachments/assets/f32d1c9a-0b0c-4a20-a8a3-8ff46b76088a" />



## Result:
Thus, the C program to convert the infix expression into postfix form using stack by following the operator precedence and associative rule is implemented successfully.
