


### 输出

#### 打印一维vector



```c++
template <typename T>
void print_vector(std::vector<T> v)
{  // 输出 vector 容器
    for (auto it = v.begin(); it != v.end(); ++it)
    {
        std::cout << *it << "  ";
    }
    std::cout << std::endl;
}
```



#### 打印二维vector

```c++
template <typename T>
void print_2d_vector(std::vector<std::vector<T> > v) // 注意>和>之间的空格, 这是代码规范之一
{  // 输出二维 vector 容器
    for (auto iti = v.begin(); iti != v.end(); ++iti)
    {
        for (auto itj = (*iti).begin(); itj != (*iti).end(); ++itj)
        {
            std::cout << *itj << "  ";
        }
        std::cout << std::endl;
    }
    std::cout << std::endl;
}
```



