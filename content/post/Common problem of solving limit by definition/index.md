---
title: Common Problem of Solving Limits by Definition
date: 2020-06-04
math: true
diagram: true
markup: mmark
---



$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

\begin{proof}
Let $\epsilon>0$, if $$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon$$ then $$\frac{1}{n^2+1}<\epsilon$$ so that $$n>\sqrt{\frac{1}{\epsilon}-1}$$

Choose $N=\left[\sqrt{\dfrac{1}{\epsilon}-1}\right]+1$ then $\forall n\geq N$, we have
$$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon$$.

Hence,

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

\end{proof}

Example **multi-line math** using the `\\` math linebreak:

```tex
$$f(k;p_0^*) = \begin{cases} p_0^* & \text{if }k=1, \\
1-p_0^* & \text {if }k=0.\end{cases}$$
```

renders as

$$f(k;p_0^*) = \begin{cases} p_0^* & \text{if }k=1, \\
1-p_0^* & \text {if }k=0.\end{cases}$$
