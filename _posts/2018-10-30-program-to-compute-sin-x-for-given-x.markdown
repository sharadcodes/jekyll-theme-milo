---
title: Program to compute sin x for given x.
date: 2018-10-30 14:59:00 Z
categories:
- C LANGUAGE PROGRAMS
- BASIC PROGRAMS
---

#### PROGRAM CODE


```c
#include <stdio.h>

int main()
{
  int i, j, n, fact, sign =  - 1;
  float x, p, sum = 0;

  printf("Enter value for x : ");
  scanf("%f", &x);
  printf("Enter value for n : ");
  scanf("%d", &n);

  for (i = 1; i <= n; i += 2)
  {
    p = 1;
    fact = 1;
    for (j = 1; j <= i; j++)
    {
      p = p * x;
      fact = fact * j;
    }
    sign =  - 1 * sign;
    sum += sign * p / fact;
  }

  printf("sin %0.2f = %f", x, sum);

  return 0;
}
```

#### OUTPUT

```
Enter value for x : 2
Enter value for n : 3
sin 2.00 = 0.666667
```