题目：
1. The Setup phase of the KZG polynomial commitment scheme involves computing commitments to powers of a secret evaluation point τ. This is called the “trusted setup" and is often generated in a multi-party computation known as the “Powers of Tau" ceremony. One day, you fnd the value of τ on a slip of paper. How can you use it to make a fake KZG opening proof?
2. Construct a vector commitment scheme from the KZG polynomial commitment scheme.
(Hint: For a vector m = (m1, . . . , mq), is there an “interpolation polynomial" I(X) such that I(i) = m[i]?)
3. The KZG polynomial commitment scheme makes an opening proof π for the relation p(x) = y. Can you extend the scheme to produce a multiproof π, that convinces us of p(xi) = yi for a list of points and evaluations (xi, yi)? (Hint: assume that you have an interpolation polynomial I(X) such that I(xi) = yi.


1、TODO

2、可以使用拉格朗日插值多项式，对于向量m=(m1,m2...mq)，令L(x) = Σ(i=1 to n) m(i) * li(x)

其中li(x)是拉格朗日基函数，li(x) = Π(j=1 to n, j!=i) (x-xj) / (xi-xj)，即li(x) === x=i?1:0

这样就实现了L(i) = m(i)

3、步骤如下：

![image](https://user-images.githubusercontent.com/26783048/224313802-a9471d39-0bae-4973-9d45-8c4c6ee31483.png)

