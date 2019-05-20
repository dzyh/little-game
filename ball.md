#include<stdio.h> 
#include<stdlib.h>
int main()
{
	
	int x_speed = 1;
	int y_speed = 1;
	int left = 0;
	int right = 20;
	int top = 0;
	int bottom = 30;
	int x=2;
	int y = 2;
	int i;
	int j;
	while (1) {
		for (i = 0; i < x; i++)
			printf("\n");
		for (j = 0; j < y; j++)
			printf(" ");

		printf("o");
		x = x + x_speed;
		y = y + y_speed;
		system("cls");
		if (x == left || x == right)x_speed = -x_speed;
		if (y == top || y == bottom)y_speed = -y_speed;

	}

	return 0;
}