---
title: PROGRAM FOR SHOWING THE IMPLEMENTATION OF CONSTRUCTORS OF IMPLICIT TYPE
date: 2018-06-18 14:41:54 Z
categories:
- BASIC OOPS PROGRAMS
- C++ LANGUAGE PROGRAMS
layout: post
---

#### PROGRAM CODE


```c
#include<iostream>
class integer
{
int m;
int n;
public:
integer(int a,int b);
void out(void)
{
std::cout << "x = " << (m/n) << '\n';
}
};

integer::integer(int x,int y)
{
m=x;
n=y;
}

int main(int argc, char const *argv[])
{
integer i(22,2);
i.out();
integer x= integer(200,2);
x.out();
return 0;
}
```
