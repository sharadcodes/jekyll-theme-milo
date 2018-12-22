---
title: PROGRAM FOR FINDING ALL PRIME NUMBERS IN A GIVEN RANGE i.e. FROM a to b
date: 2018-05-24 17:52:08 Z
categories:
- ARRAY PROGRAMS
- BASIC PROGRAMS
- C LANGUAGE PROGRAMS
layout: post
---

#### PROGRAM CODE


```c
#include<stdio.h>
void main()
{
int i,j,sum,a,b;
printf("Enter the starting of range : ");
scanf("%d",&a);
printf("Enter the ending of range : ");
scanf("%d",&b);
printf("RANGE : %d to %d\nPRIME NUMBERS : ",a,b);
for(i=a;i<=b;i++)
{
sum=0;
for(j=2;j<=i/2;j++)
{
if(i%j==0)
{
sum++;
break;
}
}
if(sum==0&&i!=1)
printf("%d ",i);
}

return 0;
}
```
