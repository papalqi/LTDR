# 模板

这里主要关心的其实是在模板领域会使用到哪些关键字

---

## decltype

**decltype 的主要作用就是推断type是什么，这在模板中是非常有用的。**  
decltype \( entity \)             \(1\)    \(since C++11\)  
decltype \( expression \)    \(2\)    \(since C++11\)

请注意，如果对象的名称带括号，则将其视为普通左值表达式，因此decltype （ x ）和decltype （（ x ））通常是不同的类型。

decltype 在声明使用标准表示法难以或不可能声明的类型时非常有用，例如与lambda相关的类型或依赖于模板参数的类型。

```cpp
    decltype ( a -> x ) y ;        // y的类型是double（声明类型） 
    decltype (( a -> x))z = y ;  // z的类型是const double＆（左值表达式）
```

而在这里，我们需要注意，参数的category不同，最后推导的结果是不同的。[^1]

1. 如果是xvalue,推导的是T&&
2. 如果是lvalue,推导的是T&
3. 如果是rvalue,推导的是T

可以使用decltype\(auto\)这种操作

```cpp
template <typename T>decltype(auto) func(T x) {return x;}
```

## template

## typename，



[^1]: 想写点什么。但是没必要，由于用不到，所以就不深入研究了，这里留着坑。

