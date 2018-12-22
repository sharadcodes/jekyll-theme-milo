---
title: Program for showing the number of passes in selection sort and the iterations
  required.
date: 2018-10-01 13:33:00 Z
layout: post
---

This program is for showing the passes in selection sort and the iterations required along with the numbers which are swapped


```cpp
#include<iostream>
using namespace std;
void swap(int &,int &);
void swap(int &a,int &b)
{
  int temp = a;
  a = b;
  b = temp;
}

void sel_sort(int arr[],int n);
void sel_sort(int arr[],int n)
{
  int i,j,min_index,count=1,x,step=1;
  for(i=0;i<n-1;i++)
  {
    min_index=i;
    for(j=i+1;j<n;j++)
    {
      if(arr[j]<arr[min_index])
      {
        swap(arr[j],arr[min_index]);
          cout<<"\nPASS "<<count<<" : ";
          count++;
            for(x=0;x<n;x++)
            {
              cout<<"\t"<<arr[x];
            }
          cout<<"\t\t"<<arr[j]<<" SWAPPED WITH "<<arr[min_index]<<"\t\tSTEP : "<<step;
    }
    else
    {
        cout<<"\n\t";
        for(x=0;x<n;x++)
        {
          cout<<"\t"<<arr[x];
        }
        cout<<"\t\t"<<"NO SWAP"<<"\t\t\t\tSTEP : "<<step;
    }
    step++;
  }
  min_index = j;
}
}

int main()
{
  int a,b,arr[40],i,n;
  cout<<"Enter the value of n : ";
  cin>>n;
  for(i=0;i<n;i++)
  {
    cout<<"Enter number "<<i+1<<" : ";
    cin>>arr[i];
  }
sel_sort(arr,n);
cout<<"\n\n\n\nSORTED ARRAY IS : ";
for(i=0;i<n;i++)
{
  cout<<"\t"<<arr[i];
}
  return 0;
}
```

### OUTPUT

```bash
Enter the value of n : 6
Enter number 1 : 67
Enter number 2 : 34
Enter number 3 : 56
Enter number 4 : 23
Enter number 5 : 45
Enter number 6 : 99

PASS 1 :        34      67      56      23      45      99              67 SWAPPED WITH 34              STEP : 1
                34      67      56      23      45      99              NO SWAP                         STEP : 2
PASS 2 :        23      67      56      34      45      99              34 SWAPPED WITH 23              STEP : 3
                23      67      56      34      45      99              NO SWAP                         STEP : 4
                23      67      56      34      45      99              NO SWAP                         STEP : 5
PASS 3 :        23      56      67      34      45      99              67 SWAPPED WITH 56              STEP : 6
PASS 4 :        23      34      67      56      45      99              56 SWAPPED WITH 34              STEP : 7
                23      34      67      56      45      99              NO SWAP                         STEP : 8
                23      34      67      56      45      99              NO SWAP                         STEP : 9
PASS 5 :        23      34      56      67      45      99              67 SWAPPED WITH 56              STEP : 10
PASS 6 :        23      34      45      67      56      99              56 SWAPPED WITH 45              STEP : 11
                23      34      45      67      56      99              NO SWAP                         STEP : 12
PASS 7 :        23      34      45      56      67      99              67 SWAPPED WITH 56              STEP : 13
                23      34      45      56      67      99              NO SWAP                         STEP : 14
                23      34      45      56      67      99              NO SWAP                         STEP : 15



SORTED ARRAY IS :       23      34      45      56      67      99
```