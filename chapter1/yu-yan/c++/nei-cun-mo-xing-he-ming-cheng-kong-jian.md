##单独编译
###头文件中的内容：
函数原型
使用#define或者const定义的符号常量
结构声明
类声明
模板声明
內联函数
###预处理器编译指令

    
```
#ifndef
#endif
```


##    存储持续性、作用域和链接性
###作用域和链接
###自动存储连续性
自动变量的初始化。
auto
register：显式的指出变量是自动的。
###静态持续变量
如果没有初始化的话，默认为0
链接性为外部的静态持续变量：在代码外面声明
连接性为内部的静态持续变量：在代码块外面，并用static
没有链接性的静态持续变量：在代码內用static
###静态持续性、外部连接性
单定义规则：
定义声明
引用声明extern
###静态持续性、内部连接性
###静态存储持续性、无连接性

说明符和限定符
mutable volatile
const全局变量如同加类static
？？？？？？？？？
函数和连接性

语言连接性
存储方案和动态分配

##名称空间
？？？？？？？？？？？
###传统的c++名称空间
声明区域
潜在作用区域
新的名称特性

名称空间示例
名称空间及前途
总结
