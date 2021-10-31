#define _CRT_SECURE_NO_WARNINGS 1

#include<stdio.h>

#include<string.h>


int main()

{

	char arr1[20] = { 0 };
  
	char arr2[] = "hello bit";
  
	strcpy(arr1, arr2);
  
	printf("%s", arr1);//打印arr1这个字符串%s 以字符串格式打印
  
	return 0;
  
}


int main()

{

	char arr[] = "hello bit";
  
	memset(arr, 'x', 5);
  

	printf("%s\n", arr);
  

	return 0;
  
}


int get_max(int x, int y)

{

	int z = x > y ? x : y;
  
	return z;
  
}


int main()

{

	int a = 10;
  
	int b = 20;
  
	//函数的调用
  
	int max = get_max(a, b);
  
	printf("max = %d\n", max);
  
	return 0;
  
}


//函数返回类型的地方写出：void，表示这个函数不返回任何值，也不需要返回


void Swap(int*pa, int*pb)

{

	int z = 0;
  
	z = *pa;
  
	*pa = *pb;
  
	*pb = z;
  
}


int main()

{

	int a = 10;
  
	int b = 20;
  
  //写一个函数，交换两个整形的变量

	printf("交换前：a=%d,b=%d\n", a, b);
  
	Swap(&a, &b);
  
	printf("交换后：a=%d,b=%d\n", a, b);
  
	return 0;
  
}
