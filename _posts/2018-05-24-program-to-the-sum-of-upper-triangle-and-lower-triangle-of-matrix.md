---
title: PROGRAM TO THE SUM OF UPPER TRIANGLE AND LOWER TRIANGLE OF MATRIX.
date: 2018-05-24 17:00:55 Z
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
int a[5][5],i,j,l,m,suml=0,sumu=0;
printf("Enter the number of rows and columns respectively in matrix : ");
scanf("%d%d",&l,&m);
if(l==m)
{
printf("\Enter elements of matrix \n\n");
for(i=0;i<l;i++)
{
for(j=0;j<m;j++)
{
printf("Enter A%d%d = ",i+1,j+1);
scanf("%d",&a[i][j]);
}
}
for(i=0;i<l;i++)
{
for(j=0;j<m;j++)
{
if(i>j)
{
suml+=a[i][j];
}
else if(i<j)
{
sumu+=a[i][j];
}
}
}
printf("Matrix is : \n");
for(i=0;i<=l-1;i++)
{
for(j=0;j<=m-1;j++)
{
printf("%d\t",a[i][j]);
}
printf("\n");
}
printf("Sum of upper triangle = %d",sumu);
printf("\nSum of lower triangle = %d",suml);
}
else
printf("Please enter a square matrix.");
return 0;
}
```
