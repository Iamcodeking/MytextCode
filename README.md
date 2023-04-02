# MytextCode
#include <stdio.h>/*********************判断重复2以上平方数121 144*************/
#include <math.h>
#include"stdlib.h"
int IsTheNumber(int n1,int n2)
{
	for (int i = n1; i <= n2; i++)
	{
		 int a = sqrt(i);int  b, number[10] = { 0 };
		if (a * a == i) /*if ((int)(a)-a == 0)*/
		{  int c=i;
			while (c)
			{
				b = c % 10;//  234%10==4  23%10==3 2%10==2
				number[b]++;//4---1  3----1   2----1
				c /= 10;//n==23  n==2   n==0
			}
			for (int ii = 0; ii <= 9; ii++)
			{
				if (number[ii] >= 2)
					printf("%d\n", i);
			}         	
		}
    }
}

int main()
{
	IsTheNumber(100,144);
system("pause");
    return 0;
}

