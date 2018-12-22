---
title: PROGRAM FOR SELECTION SORTING
date: 2018-05-24 17:06:02 Z
layout: post
categories: 
- ARRAY PROGRAMS
- C LANGUAGE PROGRAMS
---

#### PROGRAM CODE


```c
#include<stdio.h>

void swap(int*,int*);
int main()
{
int i,j,n,a[30],min;
printf("Enter the value of n :");
scanf("%d",&n);
for(i=0;i<n;i++)
{
printf("Enter number %d : ",i+1);
scanf("%d",&a[i]);
}
printf("\nArray before sorting are : ");
for(i=0;i<n;i++)
{
printf("%d ",a[i]);
}

for (i = 0;i<n-1; i++)
{
min=i;
for (j=i+1;j<n; j++)
{
if (a[j]<a[min])
{
min=j;
swap(&a[min],&a[i]);
}
}
}

printf("\nArray after sorting are : ");
for(i=0;i<n;i++)
{
printf("%d ",a[i]);
}
return 0;
}
void swap(int *x,int *y)
{
int temp;
temp=*x;
*x=*y;
*y=temp;
}
```
