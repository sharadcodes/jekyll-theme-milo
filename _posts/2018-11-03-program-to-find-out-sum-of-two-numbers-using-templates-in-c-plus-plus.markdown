---
title: Program to find out sum of two numbers using templates in C++
date: 2018-11-03 14:07:00 Z
categories:
- C++ LANGUAGE PROGRAMS
- BASIC OOPS PROGRAMS
layout: post
---

#### PROGRAM CODE

```cpp
#include<iostream>
using namespace std;

template <class T>
class sum {
  T a,b,c;
public:
  T add(T m,T n) {
    return c=(a=m)+(b=n);
  }
};

int main() {
  sum <float> o;
  cout<<"sum = a + b\n=> 3.8 + 4.2 = "<<o.add(3.8,4.2);
  return 0;
}
```

#### OUTPUT

```
sum = a + b
=> 3.8 + 4.2 = 8
```