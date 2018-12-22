---
title: SIMPLE PROGRAM FOR SHOWING THE USE OF malloc() and realloc() FUNCTIONS.
date: 2018-05-24 16:47:24 Z
categories:
- C LANGUAGE PROGRAMS
- DYNAMIC MEMORY ALLOCATION PROGRAMS
layout: post
---

#### PROGRAM CODE


```c
#include<stdlib.h>
#include<stdio.h>
#include <string.h>

int main()
{
char *x;
x=(char*)malloc(5*sizeof(char));
strcpy(x,"HELLO");
printf("The string is : %s",x);
x=(char*)realloc(x,1);
strcpy(x,"I am new");
printf("\n\nNew string after realloc is : %s",x);
return 0;
}
```
