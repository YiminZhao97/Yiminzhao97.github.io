---
layout: post
title: p values corresponding to truly null hypothesis should be uniformly distributed
categories: Statistics
---
最近看论文时，看到一个结论经常被使用——
"p values corresponding to truly null hypothesis should be uniformly distributed"。
Proof:
设检验统计量为T，T的累积分布函数（cdf）为F(T)。若为单边检验p value = G(T) = 1- F(T)；若为双边检验，p value = G(T) = 2 * (1- F(T))。显然，p value与T之间存在负相关的关系，下证在原假设正确的情况下p value服从均匀分布：
$$Pr(P \leq p) = Pr(G^{-1}(P) \leq G^{-1}(p))= Pr(T \geq t) = p $$
由此可见，p value服从均匀分布。
