# 数据类型

> 基本的数据类型

---

## void

* void 带有一组空值的类型。它是一种不完整的类型，无法初始化。
  ```cpp
    void a;//错误E0070
  ```
* 没有void数组，也没有对void的引用。
* 允许指向void的指针和返回void类型的函数。

  ```cpp
    //也就是说可以拥有void*，和void main();
  ```

  > 值得注意的是，void \*是可以指向任何的指针转换，而不是代表这是一个空的指针。
  >
  > 具体的解析，可以[参考](/chapter1/yu-yan/c++/zhi-zhen/zhi-zhen-guan-jian-zi.md)

## int

这里没有什么好说的，具体的位数参考。

## char
* signed char - 有符号的字符表示的类型。
* unsigned char- 无符号的字符。
* char -字符类型。ARM和PowerPC的默认值通常是无符号的，x86和x64的默认值通常是有符号的。通常是8位。
* wchar_t - 用于宽字符表示的类型。要求足够大以表示**任何支持**的字符代码点（在支持Unicode的系统上为32位。一个值得注意的例外是Windows，其中wchar_t是16位并且保存UTF-16代码单元）
* char16_t - 用于UTF-16字符表示的类型，要求足够大以表示任何UTF-16代码单元（16位）
* char32_t - UTF-32字符表示的类型，要求足够大以表示任何UTF-32代码单元（32位）

  
## float
* 单精度浮点类型。通常是[IEEE-754](/chapter1/yu-yan/python/ji-suan-ji-yuan-li/ieee754.md) 32位浮点类型

## double
* 双精度浮点型。通常是IEEE-754 64位浮点类型

## bool
bool - 类型，能够保存两个值之一： true或 false。sizeof （bool ）的值是实现定义的，可能与1不同。
* C和c++之类的大多数语言当中都会把非0当作TRUE，而把0当作FALSE.所以一般return 0也是非常的有玄学的。
---


#类型修饰符
>简单罗列

##long

##short

##singed

##unsigned   

