#include <stdio.h>

int main()
{
	int i, j, maxi, a[3][3], max;
	printf("input array:\n");
	a[0][0] = 0;
	for (i = 0; i < 3; i++)
		for (j = 0; j < 3; j++)
			scanf("%d", &a[i][j]);
	for (i = 0; i < 3; i++)
	{
		max = a[0][0];
		if (a[i][0] > max)	max = a[i][0];
		maxi = i;
	}
	for (j = 0;j < 3;j++)
	{
		if (a[maxi][j] > max)	max = a[maxi][j];
	}
	printf("%d/n", max);
	return(0);
}
