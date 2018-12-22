---
title: Disarium number in C++ and Python
date: 2018-09-29 19:19:00 Z
layout: post
categories:
- PYTHON
- C++ LANGUAGE PROGRAMS
---

* PROGRAM FOR DISARIUM NUMBER IN PYTHON

```python
# print((lambda x:int(x)==sum(int(d)**p for p,d in enumerate(x,1)))(input()))
[print(int(x)==sum(int(d)**p for p,d in enumerate(x,1)))for x in[input()]]
```

* PROGRAM FOR DISARIUM NUMBER IN C++

```cpp
#include <iostream>
using namespace std;

int numOfDigits(int number) 
{ 
    int digits = 0; 
    while (number) 
    { 
        number /= 10; 
        digits++; 
    } 
    return digits; 
} 
string disarium(int n, int d)
{
    int sum = 0;
    int r = n;
    int p = 1;
    for(int i = d; i > 0; i--)
    {
        for(int j = i; j > 0; j--)
        {
            p *= (n % 10);
        }
        sum += p;
        p = 1;
        n /= 10;
    }
    if(r == sum)
        return "true";
    else
        return "false";
}

int main() {
    int n;
    cin >> n;
    int d = numOfDigits(n);
    cout << disarium(n, d);
    return 0;
}
```