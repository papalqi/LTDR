UTF-8 字符文字；


内联变量 (inline variables)：允许在头文件中定义变量；
    >简而言之，如果你需要声明在编译单元之间共享的全局变量，在头文件中将它们声明为内联变量是很简单的，并且避免了前C ++ 17解决方法的问题

在 if 和 switch 语句内可以初始化变量；

结构化绑定 (Structured Binding)：for (auto [key,value] : my_map) {…}；

类模板参数规约 (Class Template Argument Deduction)：用 pair p{1, 2.0}; 替代 pair<int, double>{1, 2.0};；

使 static_assert 的文本信息可选；static_assert with no message


* 删除 trigraphs
    >thrgraph是C/C++ 为了照顾老一辈的"无产阶级革命家"而出现的,当时他们的条件极其艰苦，键盘上缺了很多        键,无法输入以下九个字符:
      # \ ^ [ ] { } | ~ 由此推才出现了 trigraph .

在模板参数中允许使用 typename（作为替代类）；

来自 braced-init-list 的新规则用于自动推导；

嵌套命名空间的定义，例如：使用 namespace X::Y { … } 代替 namespace X { namespace Y { … }}；

允许命名空间和枚举器的属性；

新的标准属性：[[fallthrough]], [[maybe_unused]] 和 [[nodiscard]]；

对所有非类型模板参数进行常量评估；

* Fold 表达式,折叠表达式，用于可变的模板；
    >C++11 提供了可变模板参数包, 使函数可以接受任意数量的参数. 但在 C++11 中展开参数包稍显麻烦, 而 C++17 的折叠表达式使得展开参数包变得容易, 其基本语法是使用 (...) 的语法形式进行展开.

* 结构化的绑定声明，现在允许 auto [a, b] = getTwoReturnValues();
    > 不太用的到

在某些情况下，确保通过编译器进行 copy elision（Guaranteed copy elision by compilers in some cases）；

一些用于对齐内存分配的扩展；

构造函数的模板推导，允许使用 std::pair(5.0, false) 代替 std::pair<double,bool>(5.0, false)；

__has_include，允许由预处理程序指令检查头文件的可用性；

__cplusplus 的值更改为 201703L；
78737012 
