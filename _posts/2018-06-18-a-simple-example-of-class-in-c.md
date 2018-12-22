---
title: A SIMPLE EXAMPLE OF CLASS IN C++
date: 2018-06-18 14:20:18 Z
categories:
- BASIC OOPS PROGRAMS
- C++ LANGUAGE PROGRAMS
layout: post
---

#### PROGRAM CODE


```c
#include<iostream>
class student
{
float marks;
public:
void putMarks(float m)
{
marks = m;
}
void showMarks(void)
{
std::cout << marks << '\n';
}
};
int main(int argc, char const *argv[]) {
float x;
student s1;
std::cout << "ENTER THE MARKS : ";
std::cin >>x;
s1.putMarks(x);
std::cout << "YOU ENTERED : " ;
s1.showMarks();
return 0;
}
```
