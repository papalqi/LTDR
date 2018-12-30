#value category
这里的value category 和变量的类型（type）是完全不同的概念,具体的中文翻译不太清楚，所以这里就直接使用英文。
对于c++的每一个表达式（运算符及其操作数、文字、变量名等），都有一个value category.
其主要分为以下三种
* glvalue（“广义”lvalue）
* prvalue
* xvalue
在c++历史的长河当中，经过了很多的修改，所以还有其它的概念
* rvalue    
* lvalue
## glvalue