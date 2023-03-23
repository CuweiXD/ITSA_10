# 題目10. 輾轉相除法
### 問題描述：
給定二個正整數，利用輾轉相除法求其最大公因數。

### 輸入說明：
給定二個正整數

### 輸出說明：
輸出最大公因數

### 範例：
#### 輸入範例:
300 250

#### 輸出範例:
50

### 解答
```
#include <iostream>
using namespace std;

int f(int(x))
{

    if (x == 0 || x == 1) {

        return x + 1;
    }

    else if (x > 1) {
        return f(x - 1) + f(x / 2);
    }

}
int main()
{
    int x;
    cin >> x;
    cout << f(x) << endl;
}
```

