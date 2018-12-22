---
title: AN EXAMPLE OF ARRAY OF OBJECTS OF A CLASS
date: 2018-06-18 14:39:35 Z
categories:
- BASIC OOPS PROGRAMS
- C++ LANGUAGE PROGRAMS
layout: post
---

#### PROGRAM CODE


```c
#include<iostream>
class MY{
int x;
public:
void put(void);
void out(void);
};
void MY :: put(void)
{
std::cout << "ENTER THE VALUE x : ";
std::cin >> x;
}
void MY :: out(void)
{
std::cout << "X = "<<x << '\n';
}

int main() {
MY OB[5];
int i;
for (size_t i = 0; i < 5; i++) {
OB[i].put();
}
for (size_t i = 0; i < 5; i++) {
OB[i].out();
}
return 0;
}
```
