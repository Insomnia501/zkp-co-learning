1、TODO

2、可以使用拉格朗日插值多项式，对于向量m=(m1,m2...mq)，令L(x) = Σ(i=1 to n) m(i) * li(x)

其中li(x)是拉格朗日基函数，li(x) = Π(j=1 to n, j!=i) (x-xj) / (xi-xj)，即li(x) === x=i?1:0

这样就实现了L(i) = m(i)

3、步骤如下：

![image](https://user-images.githubusercontent.com/26783048/224313802-a9471d39-0bae-4973-9d45-8c4c6ee31483.png)

