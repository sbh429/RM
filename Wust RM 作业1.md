# 作业

1. 数组反转

```cpp
#include <iostream>
#include <vector>
using namespace std;

int main()
{
int n;
cin>>n;
if(n==0)
    cout<<"n不可为0"<< endl;
    return 0;
vetor<int> arr(n);
int *p=arr.data();
for (int i = 0;i < n;i++)
	cin >> *(p+i);// 录入数据
for (int p = 0;p <( n/2);p++)
{
	int q = n - 1 - p;
	int t = arr[p];
	arr[p] = arr[q];
	arr[q] = t;
}//交换数组
for (int i = 0;i < n;i++)
{
	cout << *(p+i) << " ";9
}

return 0;
}

2.爬楼梯

```cpp
#include <iostream>
using namespace std;

int stair(int n)
{
	if (n<=2)
	{
		return n;
	}
	return stair(n-1)+stair(n-2)//递归函数
}
int main()
{
	int n;
	cin >> n;
	cout << "递归" << endl;
	cout << "有" << stair(n) << "种爬法" << endl;
}
//想不出来迭代 感觉迭代好麻烦

3.二叉树
```cpp
