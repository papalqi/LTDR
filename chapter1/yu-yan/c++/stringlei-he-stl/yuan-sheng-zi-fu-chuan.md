#原生字符串（raw string literals）
很多时候，当我们只需要一行字符串的时候，字符串转义往往成了一个负担，和写和读都带了很大的不便。例如，对于如下路径"C:\Program Files\Microsoft.NET\ADOMD.NET"，我们必须把它写成如下形式：

    string path = "C:\\Program Files\\Microsoft.NET\\ADOMD.NET";

可能你会说这个并没有多大影响，下面这个正则表达式的例子呢？你能看出来原文到底是什么吗？

    string exp = "('(?:[^\\\\']|\\\\.)*'|\"(?:[^\\\\\"]|\\\\.)*\")|";

在C#中，我们可以通过@关键字来取消字符串转义。现在，在C++ 11中，也增加了这样的语法。对于前面的例子，它的非转义形式为：

    string path = R"(C:\Program Files\Microsoft.NET\ADOMD.NET)";

从上面的例子中可以看出，它的语法格式如下：

字符串前加'R'前缀
字符串首尾加上括号()
它的语法格式比C#的@前缀要稍微复杂点，不过这个复杂也有复杂的好处，那就是字符串里面可以带引号，例如：

    string path = R"(this "word" is escaped)";

