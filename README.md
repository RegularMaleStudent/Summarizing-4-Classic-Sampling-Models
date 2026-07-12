# Summarizing-4-Classic-Sampling-Models

| 是否放回 | 是否有序 | 对应分布 | 样本空间大小 | 概率计算公式 | 记号 |
|---|---|---|---|---|---|
| 有放回 | 有序 | — | 可重排列 $N^n$ | i.i.d. 概率连乘 | — |
| 有放回 | 无序 | 二项分布 / 多项分布 | 可重组合 $H_N^n = \binom{N+n-1}{n}$（二项时 $N=2$） | $\dfrac{n!}{n_1!\cdots n_N!}\,p_1^{n_1}\cdots p_N^{n_N}$ | 二项 $B(n,p)$ / 多项 $M(n;p_1,\dots,p_N)$ |
| 不放回 | 有序 | — | 排列 $A_N^n = \dfrac{N!}{(N-n)!}$ | 逐次条件概率连乘 | — |
| 不放回 | 无序 | 超几何 / 多元超几何 | 组合 $\binom{N}{n}$ | $\dfrac{\binom{M}{k}\binom{N-M}{n-k}}{\binom{N}{n}}$ | 超几何 $H(N,M,n)$ / 多元超几何 $MH(N,\mathbf{K},n)$ |
