---
title: PROGRAM FOR CONVERTING DECIMAL TO BINARY
date: 2018-08-02 16:04:15 Z
categories:
- BASIC PROGRAMS OF C++
- C++ LANGUAGE PROGRAMS
layout: post
---

#### PROGRAM CODE


```c
#include<iostream>
class conversion {
public:
int rem,dec,i=0,binary[100];
void d_to_b(void);
};
void conversion :: d_to_b(void)
{
while(dec!=0)
{
rem=dec%2;
dec=dec/2;
binary[i]=rem;
i++;
}
i=i-1;

std::cout << "Binary number is : ";
while(i>=0)
{
std::cout<<binary[i];
i--;
}

}

int main()
{
conversion number;
std::cout << "Enter the decimal number : ";
std::cin >> number.dec;
number.d_to_b();
return 0;
}
```
