# Cpractice

#define _CRT_SECURE_NO_WARNINGS 1
#include <stdio.h>
#include <windows.h>
//三个数排大小
void swap(int *x, int *y)
{
	int tmp = *x;
	*x = *y;
	*y = tmp;
}

int main()
{
	int a = 0;
	int b = 0;
	int c = 0;
	scanf("%d%d%d", &a, &b, &c);
	if (a > b)
	{
		swap(&a, &b);
	}
	if (a > c)
	{
		swap(&a, &c);
	}
	if (b > c)
	{
		swap(&b, &c);
	}
	printf("%d %d %d \n", a, b, c);

	system("pause");
	return 0;
}


#include <stdio.h>
#include <windows.h>

//求最大公倍数\最小公倍数
int main()
{
	int num1 = 0;
	int num2 = 0;
	scanf("%d%d", &num1, &num2);
	int number1 = num1;
	int number2 = num2;
	int tmp;
	if (tmp = number1%number2)
	{
		number1 = number2;
		number2 = tmp;
	}
	printf("最大公约数是：%d\n", number2);

	printf("最小公倍数是：%d\n", (num1*num2) / number2);

	system("pause");
	return 0;
}

#include <stdio.h>
#include <windows.h>
#include <string.h>

大写-小写互换，数字不输出  如：ABC123def-abcDEF
int main()
{
	char arr[] = "abad123EF";
	int i = 0;
	for (i = 0; i < strlen(arr); i++)
	{
		if (arr[i] >= 'a'&&arr[i] <= 'z')
		{
			arr[i] = arr[i] - 32;

		}
		else if (arr[i] >= 'A'&&arr[i] <= 'z')
		{
			arr[i] = arr[i] + 32;
		}
		else
		{
			arr[i] = 0;

		}
	}
	printf("%s\n", arr);
	system("pause");
	return 0;
}

#include <stdio.h>
#include <windows.h>

int main()
{
	int ch = 0;
	while ((ch = getchar()) != EOF)
	{
		if (ch >= 'a'&&ch <= 'z')
		{
			putchar(ch-32);
		}
		else if (ch >= 'A'&&ch <= 'Z')
		{
			putchar(ch + 32);
		}
		else if (ch >= '0'&&ch <= '9')
		{
			;
		}
		else
		{
			putchar(ch);
		}
	}
	system("pause");
	return 0;
}




