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

int main()
{
    int x, y;
    cin >> x >> y;
    while (x != 0 && y != 0) {

        if (x >= y) {
            x = x % y;
        }
        else if (y > x) {
            y = y % x;
        }

    }

    if (x > y) {
        cout << x << endl;

    }
    else {
        cout << y << endl;
    }

}
```

