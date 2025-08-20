# EX3 Implementation of Tower of Hanoi
## DATE:
## AIM:
To write a C program to implement Tower of Hanoi.

## Algorithm
1. Start with n disks on the source rod.
2. Move n-1 disks from source rod to auxiliary rod using the target rod.
3. Move the nth disk from source rod to target rod.
4. Move the n-1 disks from auxiliary rod to target rod using the source rod.
5. Repeat recursively until all disks are moved to the target rod.

## Program:
```
/*
Program to implement Tower of Hanoi
Developed by: Swetha S
RegisterNumber: 212222230155
*/
```

```
/*
#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
  // Write your code here 
  if(n>0)
  {
      TOH(n-1,x,z,y);
      printf("%c to %c\n",x,y);
      TOH(n-1,z,y,x);
  }
}
int main()
{
   // Write your code here 
   int n;
   scanf("%d",&n);
   TOH(n,'A','B','C');
}
*/
```

## Output:
<img width="307" height="686" alt="image" src="https://github.com/user-attachments/assets/1d289e27-382d-4bf8-bd09-9879334ba830" />



## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
