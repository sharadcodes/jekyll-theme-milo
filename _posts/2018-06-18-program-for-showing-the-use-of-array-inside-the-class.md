---
title: PROGRAM FOR SHOWING THE USE OF ARRAY INSIDE THE CLASS
date: 2018-06-18 14:37:18 Z
categories:
- BASIC OOPS PROGRAMS
- C++ LANGUAGE PROGRAMS
layout: post
---

#### PROGRAM CODE


```c
#include<iostream>
// CLASS DECLARATION
class first
{
int x[5];
public:
void put(void);
void out(void);
};
//MEMBER VARIABLE DEFINITION
void first:: put() {
for (int i = 0; i < 5; i++) {
int input;
std::cout << "ENTER THE VALUE FOR x["<<i<<"] : ";
std::cin >> input;
x[i]=input;
}
}
void first:: out(void) {
for (int i =0; i < 5;i++) {
std::cout << "\nVALUR OF x["<<i<<"] = "<<x[i] << '\n';
}
}

int main(int argc, char const *argv[]) {
first obj;
obj.put();
obj.out();
return 0;
}
```
