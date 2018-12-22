---
title: Program for showing the number of passes in bubble sort and the iterations
  required.
date: 2018-10-01 13:41:00 Z
---

This program is for showing the passes in bubble sort and the iterations required along with the numbers which are swapped

```cpp
#include<iostream>
using namespace std;
void swap(int &,int &);
void swap(int &a,int &b)
{
int temp;
temp = a;
a = b;
b = temp;
}
int main()
{
int i,j,n,a[50],k,pass=1;
cout<<"Enter the value of n : "; // n is the number of elements in the array
cin>>n;
for(i=0;i<n;i++)
{
	cout<<"Enter number "<<i+1<<" : ";
	cin>>a[i];
}
cout<<"\n\nBUBBLE SORT \n\n";
cout<<"\nINDEX NUMBER : ";
for(i=0;i<n;i++)
{
cout<<"\t"<<i;
}
cout<<endl;
for(i=0;i<n-1;i++)
{
	for(j=0;j<=n-i-1;j++)
	{
	if(a[j]>a[j+1])
	{
		swap(a[j],a[j+1]);

		cout<<"\nPASS "<<pass<<" :\t";
		for(k=0;k<n;k++)
		{
		cout<<a[k]<<"\t";
		}
	  cout<<"\t"<<a[j]<<" at index "<<j+1<<" swapped with "<<a[j+1]<<" at index "<<j;
		cout<<"\n\n";

		pass++;
	}
	}
}
return 0;
}
```

### OUTPUT

```bash
Enter the value of n : 6
Enter number 1 : 34
Enter number 2 : 23
Enter number 3 : 45
Enter number 4 : 6
Enter number 5 : 453
Enter number 6 : 231


BUBBLE SORT


INDEX NUMBER :  0       1       2       3       4       5

PASS 1 :        23      34      45      6       453     231             23 at index 1 swapped with 34 at index 0


PASS 2 :        23      34      6       45      453     231             6 at index 3 swapped with 45 at index 2


PASS 3 :        23      34      6       45      231     453             231 at index 5 swapped with 453 at index 4


PASS 4 :        23      6       34      45      231     453             6 at index 2 swapped with 34 at index 1


PASS 5 :        6       23      34      45      231     453             6 at index 1 swapped with 23 at index 0
```