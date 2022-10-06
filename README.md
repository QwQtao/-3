# -3
for循环练习题（三）两边缩减找下标

#include<windows.h>//休息一秒（1000）
#include<stdlib.h>//system函数

int main()
{
	//wlecome to bit!!!!!!
	//####################
	//w##################!
	//we################!!
	//wel##############!!!
	//...
	//wlecome to bit!!!!!!

	//char arr[]="abc";
	//[a b c \0]
	// 0 1 2  3
	//因为最后一个！后面有空格（\n），所以得4-2，才能得到c=2；
	char arr1[] = "welcome to bit!!!!!!";
	char arr2[] = "####################";
	int left = 0;
	//int right =sizeof(arr1)/sizeof(arr1[0])-2;//err
	int right = strlen(arr1) - 1;

		while (left <= right)
		{
			arr2[left] = arr1[left];
			arr2[right] = arr1[right];
			printf("%s\n", arr2);
			//休息一秒，能直观感受
			Sleep(1000);
			system("cls");//执行系统命令的一个函数、、、//cls——清空屏幕
			left++;
			right--;
		}
		printf("%s\n", arr2);
	return 0;
}

