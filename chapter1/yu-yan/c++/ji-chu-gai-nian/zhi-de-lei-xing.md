# value category

> 这里的value category 和变量的类型（type）是完全不同的概念,具体的中文翻译不太清楚，所以这里就直接使用英文。  
> 对于c++的每一个表达式（运算符及其操作数、文字、变量名等），都有一个value category.  
> 其主要分为以下三种
>
> * glvalue（“广义”lvalue）
> * prvalue
> * xvalue
>   在c++历史的长河当中，经过了很多的修改，所以还有其它的概念
> * rvalue    
> * lvalue

---

## lvalue\(左值\)

具体的含义就不再赘述了

* 可以采用左值的地址     ＆++ i和＆std :: endl
* 可修改的左值可以用作内置赋值和复合赋值运算符的左操作数

## rvalue（右值）

* 没有地址
* rvalue不能用作内置赋值或复合赋值运算符的左操作数。
* 可以使用rvalue 初始化const左值引用，在这种情况下，由rvalue标识的对象的生命周期被延长，直到引用的范围结束。
* 可以使用rvalue初始化rvalue引用，在这种情况下，由rvalue标识的对象的生命周期被延长，直到引用的范围结束。
* 当用作函数参数并且当函数的两个重载可用时，一个采用rvalue引用参数而另一个采用lvalue引用const参数，rvalue绑定到rvalue引用重载（因此，如果复制和移动构造函数都可用） ，一个rvalue参数调用移动构造函数，同样使用复制和移动赋值运算符）

## glvalue

这里一定是左值或者X值

* 可以进行隐式转换
* 可以多态

## prvalue

* 与右值相同（下图）。
* prvalue不能是多态的：它标识的对象的动态类型始终是表达式的类型。
* 非类非数组prvalue不能是cv限定的（const and volatile）。（注意：函数调用或强制转换表达式可能会导致非类cv限定类型的prvalue，但会立即删除cv-qualifier。）
* prvalue不能具有不完整的类型（例如类型为void）
* prvalue不能具有抽象类类型或其数组。

## xvalue

* 与右值相同。
* 与glvalue相同、

---

目前水平比较初级，没有用到这方面的实际问题，所以理解的不深。

