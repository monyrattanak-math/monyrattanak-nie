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

Correciones:

Proof 1: Using definition for all $\epsilon>0$

Given $\epsilon>0$, then

$$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon\Leftrightarrow\frac{1}{n^2+1}<\epsilon\Leftrightarrow n^2>\frac{1}{\epsilon}-1$$ 

Define

$$ N=
\begin{cases}
\left[\sqrt{\dfrac{1}{\epsilon}-1}\right]+1 & \text{ if }0<\epsilon<1 \\
1 & \text{ if } \epsilon\geq 1
\end{cases}
$$

then $$\forall n\geq N$$, we have

$$ n^2\geq N^2>\frac{1}{\epsilon}-1 \Rightarrow
\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon$$

Hence,

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

Proof 2: Using small $\epsilon$ and extend to all $\epsilon>0$

Let $0<\epsilon\leq 1$, then

$$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon\Leftrightarrow\frac{1}{n^2+1}<\epsilon\Leftrightarrow n^2>\frac{1}{\epsilon}-1>0\Leftrightarrow n>\sqrt{\frac{1}{\epsilon}-1}$$

Choose $$N_\epsilon=\left[\sqrt{\dfrac{1}{\epsilon}-1}\right]+1$$ then $$\forall n\geq N_\epsilon $$, we have

$$ n>\sqrt{\frac{1}{\epsilon}-1}\Rightarrow\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon $$

If $$\epsilon> 1$$, choose $N=N_1$ then $$\forall n\geq N$$, we have
$$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<1<\epsilon$$.

Hence,

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

Proof 3: Using archimedean property

Given $\epsilon>0$. By archimedean property, there exists $N\in\N$ such that $\frac{1}{N}<\epsilon$. Then for all $n\geq N$, we have

$$
\Big\vert\frac{n^2}{n^2+1}-1\Big\vert=\frac{1}{n^2+1}\leq \frac{1}{N^2+1}\leq\frac{1}{N}<\epsilon.
$$

Hence,

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$
