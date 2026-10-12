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
for (int i = 0;i < n;i++)
	cin >> arr[i];// 录入数据
for (int p = 0;p <( n/2);p++)
{
	int q = n - 1 - p;
	int t = arr[p];
	arr[p] = arr[q];
	arr[q] = t;
}//交换数组
for (int i = 0;i < n;i++)
{
	cout << arr[i] << " ";9
}

return 0;
}
```
2.