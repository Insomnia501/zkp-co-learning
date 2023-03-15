题目：https://hackmd.io/@gubsheep/Hy57lluOs

1.

1)对于三染色问题如果可以看相邻边的话，就可以通过多次查看来获取“哪两个节点是同一颜色”，这就是一个非零知识系统（在拓扑结构可变/不可变均会泄露信息）

2)该公式有误，应为(1-1/E)^n

2. TODO

3. 

1)Explain why you need to generate and save a “secret” value.
 - 因为我们需要secret value作为私钥来生成群签名


3)Log into the same zkmessage account, from a different browser or computer. Explain why zkmessage can’t just use a simple “username/password” system like most social apps.
 - 用户名系统有被盗窃账号的风险，群签名的方式可以保障私钥信息安全，除非盗窃者知道全部私钥信息。
