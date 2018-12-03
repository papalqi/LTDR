#string类
##构造字符串
移动构造函数，编译器可用它而不是复制构造函数，来优化性能，在18章“移动语义和右值引用”讨论这个问题。
##string类输入
string stuff;
getline(info,100,':');
char info[100]
cin.getline(info,100);


cin.operator>>(fname)
operator>>(cin,lname);
这两个都有一些限制，第一个限制就是string对象允许的最大允许长度，由常量string::npos
另一个限制因素是程序可以使用的内存量。

1到达文件尾，输入流的eofbit将被设置，这意味着方法fail（）和eof（）都将返回true；
2遇到分界字符。将分界字符从输入流中删除，但不存储它。
3.达到最大值，将设置输入流的failbit，这意味着fail（）将返回true
##使用字符串

##string还提供了哪些功能
删除字符串的部分或者全部内容
用一个字符串的部分或全部内容替换另一个字符串的部分或全部内容
等等，
##字符串种类
#智能指针模板类
、三个帮助管理内存动态分配的只能指针模板，如果指针是对象，则就可以调用析构函数。
   auto_ptr\unique_ptr\shared_ptr

##使用智能指针
必须包含头文件memory
auto_ptr<double>ap(new double)，new double是new返回的指针，指向新分配的内存块，
##有关智能指针的注意事项
赋值：两次删除对象，同样适用于复制构造函数。
定义赋值运算符，进行深刻复制。
建立所有权，只能有一个智能指针可拥有。这是auto_ptr的策略



如果源unique_ptr是一个临时右值，编译器允许这么做。如果源unique_ptr将存在一段时间，编译器将禁止这么做。
如何能区分安全或者不安全呢，答案是它使用了c++11新增的移动构造函数和右值引用


需不需要多个指向同一个对象的指针。
BOOST库

STL提供了一组表示容器，迭代器，函数对象，和算法的模板。STL不是面向对象的编程，而是一种不同的编程模式。泛型编程，这使得STL的功能和方法方面都很有趣。

vector<int>ratings(5);与string类相识，各种STL容器模板都接受一个可选的模板参数，该参数指定使用哪个分配器对象来管理内存。

size(),swap(),begin(),end(),
什么是迭代器：是一个广义指针，事实上，它可以是指针，也可以是一个可对其执行类似指针的操作，
定义迭代器：vector<double>scores;vector<double>::iterator pd; pd=scoers.begin();
当然可以使用c++的自动类型推断 auto pd=score.begin();
push_back();erase();insert()

定义了一个适用于所有容器类的非成员函数find（）
一般来说，特定算法的效率比通用算法高。
for_each(books.begin(),books.end(),showreview);
random_shuffle(books.begin(),books.end());
sort();
##基于范围的for循环
for(double x: price)
x.ssss;


泛型编程关注的是算法。抽象和创建可重用代码。
泛型编程旨在编写独立于数据类型的代码。

实际上，作为一种编程风格，最好避免直接使用迭代器，而应尽可能使用STL函数。
为何使用迭代器
##迭代器的类型
输入迭代器：需要这个的都不会修改容器的值，是单向的，不能倒退
输出迭代器：不能读，只能写
正向迭代器：总是按相同顺序遍历一系列值。使得多次通行算法成为可能。
双向迭代器：具有正向的所有特性。
随机访问迭代器

##迭代器的层次结构
##函数对象
?????????????????????????????????
预定义函数符
自定义函数符合函数适配器
##算法
算法组
算法的通用特征
STL和string类
函数和容器方法
使用STL
##其他库
vector，valarray，array
模板 initializer_list
使用initializer_list
