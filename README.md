# PTA_7-6
# 混合类型数据格式化输入
# 本题要求编写程序，顺序读入浮点数1、整数、字符、浮点数2，再按照字符、整数、浮点数1、浮点数2的顺序输出。

# 输入格式：输入在一行中顺序给出浮点数1、整数、字符、浮点数2，其间以1个空格分隔。

# 输出格式：在一行中按照字符、整数、浮点数1、浮点数2的顺序输出，其中浮点数保留小数点后2位。

```cpp
#include<iostream>
#include<iomanip>
using namespace std;

int main() {
	float float1, float2;
	int integer;
	char character;

	cin >> float1 >> integer >> character >> float2;  //按照类型输入
	cout << character << " " << integer << " " >>
     fixed << setprecision(2) << float1 << " " << float2 << endl;  //按照要求类型顺序输出，确保浮点数保留小数点后两位

	return 0;
}