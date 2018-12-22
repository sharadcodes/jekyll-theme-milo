---
title: Program for finding factorial using pointers
date: 2018-09-29 15:47:00 Z
layout: post
---

C language program for finding factorial using pointers.

```c
#include<stdio.h>
float f(int);

int main()
{
    int a;
    printf("Enter the number : ");
    scanf("%d",&a);
    printf("Factorial of %d is %f",a,f(a));
    return 0;
}
float f(int x)
{
    float sum=1,*p;
    while(x>0)
        {
            sum=sum*x;
            x--;
        }
    p=&sum;
    return *p;
}
```