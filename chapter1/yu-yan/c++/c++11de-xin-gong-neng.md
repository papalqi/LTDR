# c++11功能

## 新类型

* long long，unsigned long long，支持64位的整形

* char16\_t char32\_t支持16位和32位的字符表示。（[其它参见](/chapter1/yu-yan/python/bian-cheng-yu-yan-zhong-de-wei-shu.md)）

* 还新增了[原生字符串](/chapter1/yu-yan/c++/stringlei-he-stl/yuan-sheng-zi-fu-chuan.md)


## 统一的初始化

扩大了大括号的列表的使用范围。也可用于new，关于初始化的内容，参见

* 缩窄

初始化列表可以防止缩窄，禁止将树脂赋予无法存储它的数值变量。

* std::initializer\_list

  * 可以把它用作构造函数的参数。

  * 列表中的元素必须是同一种类型或者可以变成同一种类型。

## 声明

* auto

* decltype 将变量的类型声明为表达式指定的类型 decltype（x）y

* 返回类型后置， 用来指定模版函数的返回类型

* 模版别名

  *  using=

  *  以前提供了typedef

using可以用于模版部分具体化

* nullptr

## 智能指针

## 异常规范方面的修改

* 指出不回引发异常 noexcept

## 作用域内枚举

## 对类的修改

* 显示转换运算符：explicit

* 类內成员初始化

## 模版和STL方面的修改

* 基于范围的for循环

      for（auto x=prices）

* 新的STL容器

* 新的STL方法

* valarray升级

* 摒弃export

*尖括号

## 右值引用

## 移动语义和右值引用

* 为什么需要移动语义

* 只是调整记录而不是复制

* 一个移动示例

* 移动构造函数解析

* 赋值

## 新的类功能

*特殊的成员函数

* 默认的方法和禁用的方法

* 委托构造函数

* 继承构造函数

* 管理虚方法

## lambda函数

* 比较函数指针，函数符和lambda函数

* 为何使用lambada

## 包装器

* 包装齐function及模版的低效型

* 修复问题

* 其他方式

## 可变参数模板

* 模板和函数参数包

* 展开参数包

* 在可变参数模板函数中使用递归

## c++新增的其他功能

* 并行编程

* 新增的库

* 低级编程

* 杂项

## 语言变化

* boost项目

* TR1

* 使用BOOST

## 接下来的任务



