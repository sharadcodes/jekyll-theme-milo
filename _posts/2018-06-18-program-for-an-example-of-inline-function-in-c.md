---
title: PROGRAM FOR AN EXAMPLE OF INLINE FUNCTION IN C++
date: 2018-06-18 14:22:30 Z
categories:
- BASIC OOPS PROGRAMS
- C++ LANGUAGE PROGRAMS
layout: post
---

#### PROGRAM CODE


```c
#include<iostream>
void in(int);
int main(int argc, char const *argv[]) {
in(3);
return 0;
}
inline void in(int x)
{
std::cout << x << '\n';
}
```
