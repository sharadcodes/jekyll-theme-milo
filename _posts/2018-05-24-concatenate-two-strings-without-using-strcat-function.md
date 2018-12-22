---
title: CONCATENATE TWO STRINGS WITHOUT USING strcat() FUNCTION
date: 2018-05-24 17:48:47 Z
categories:
- C LANGUAGE PROGRAMS
- STRING PROGRAMS
layout: post
---

#### PROGRAM CODE


```c
#include<string.h>
#include<stdio.h>
void main()
{
char s1[20],s2[20];
int i,j=0;
printf("Enter first string : ");
gets(s1);
printf("Enter string second : ");
gets(s2);
i=strlen(s1);
while(j<strlen(s1))
{
s1[i+j]=s2[j];
j++;
}
printf("String after con is : %s",s1);
return 0;
}
```
