#### [剑指 Offer 05. 替换空格](https://leetcode-cn.com/problems/ti-huan-kong-ge-lcof/)

> 请实现一个函数，把字符串 `s` 中的每个空格替换成"%20"。

**示例 1：**

```
输入：s = "We are happy."
输出："We%20are%20happy."
```

**限制：**

```
0 <= s 的长度 <= 10000
```



* **利用c++ STL string的特性进行简单的模拟即可**

```c++
class Solution {
public:
    string replaceSpace(string s) {
        string res;
        for(auto ch:s){
            if(ch==' '){
                res += "%20";
            }else{
                res += ch;
            }
        }
        return res;
    }
};
```


