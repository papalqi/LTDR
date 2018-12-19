#数学期望（Expectation）
>在概率论和统计学中是试验中每次可能结果的概率乘以其结果的总和，是最基本的数学特征之一。它反映随机变量平均取值的大小。
通常是使用E(X)来标识

###1定义
[对于离散型随机变量](/shu-xue-ji-chu/gai-lv-lun/li-san-xing-sui-ji-bian-liang.md)：$$E(x)=\sum_{k=1}^{\infty}{x_{k}p_{k}}$$

[对于连续性随机变量](/shu-xue-ji-chu/gai-lv-lun/lian-xu-xing-sui-ji-bian-liang.md)：$$E(x)=\int_{-\infty}^{\infty}{xf(x)}dx$$
###2性质
####2.1线性
先看离散的
$$\begin{align*} E(X+Y)&=\sum_{i,j} (x_{i}+y_{j})p_{ij}\\ &=\sum_{i} x_{i}\sum_{j}p_{ij}+\sum_{j}y_{j}\sum_{i}p_{ij}\\ &=E(X)+E(Y) \end{align*}$$
连续的情况类似
$$E(X+Y)=\int\int (x+y)f(x,y)dxdy=E(X)+E(Y)$$
[why](/shu-xue-ji-chu/gao-deng-shu-xue/ji-fen/ji-fen-de-xing-zhi.md)
####2.2常数倍
$$E(aX)=aE(X)$$ 
####2.3 若X∼f(x),导出的新随机变量Y=g(X)
$$E(Y)=\int_{-\infty}^{+\infty}g(x)f(x)dx$$
####2.4如果独立
$$E(XY)=E(X)E(Y)$$


[对于连续性随机变量](/shu-xue-ji-chu/gai-lv-lun/lian-xu-xing-sui-ji-bian-liang.md)：$$E(x)=\int_{-\infty}^{\infty}{xf(x)}dx$$


###3思考
因为实际中[概率密度函数](/shu-xue-ji-chu/gai-lv-lun/gai-lv-mi-du-han-shu.md)很难求，期望往往是其中一个未知的参数。
####3.1数学期望和均值（mean）
均值，其实是样本的特性，而期望，是一种加权平均
####3.2对于某些辨析
[请参考这里的解释](/shu-xue-ji-chu/gai-lv-lun/fang-cha.md)
####3.3数学期望的几何意义
如果想象成为重心几何，期望其实就是**重心**
