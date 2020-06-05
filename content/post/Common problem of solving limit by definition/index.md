---
title: Common Mistake of Solving Limits of Sequence by Definition
date: 2020-06-04
math: true
diagram: true
markup: mmark
---
We present a mistake some students and teachers made when solving limit of sequence by definition. Consider the following example.

Example 1: Prove by definition that

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

The following proof are used by some students and teacher.

Let $\epsilon>0$, if $$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon$$ then $$\frac{1}{n^2+1}<\epsilon$$ so that $$n>\sqrt{\frac{1}{\epsilon}-1}$$

Choose $N=\left[\sqrt{\dfrac{1}{\epsilon}-1}\right]+1$ then $\forall n\geq N$, we have
$$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon$$.

Hence,

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

The error in the proof is that the way they choose the value N. N is not defined if $$\epsilon$$ is too big. This tiny mistake always made when they are ignore or don't understand very well the definition of the limit, and usually think of $$\epsilon$$ choosen being small enough. We can only prove for sufficently small $$\epsilon$$ if we already proof or understand the equivalence between the two.

We provide 3 different proof for the above problem. The reader should compare these 3 ways with each other and proof above.

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

Given $\epsilon>0$. By archimedean property, there exists $N\in\mathbb{N}$ such that $\frac{1}{N}<\epsilon$. Then for all $n\geq N$, we have

$$
\Big\vert\frac{n^2}{n^2+1}-1\Big\vert=\frac{1}{n^2+1}\leq \frac{1}{N^2+1}\leq\frac{1}{N}<\epsilon.
$$

Hence,

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

We can see that in proof 3, we don't need to solve for N. By definition of the limit, we just want to know whether exists N or not. There are 2 version of the archimedean property.

Version 1: For any real number x, there is a natural number n such that $$x<n$$.

Version 2: For any real number a and b, there is a natural number such that $$a<nb$$.

Now, we give another example and solve it using the archimedean property. The reader can try to solve it using way 1 or way 2 above and compare.

Example 2: Prove by definition that

$$
\lim_{n\to\infty}{\frac{n}{\sqrt[3]{n^3+1}}}=1.
$$

Proof: For all $n=1,2,\cdots$, we have

$$
\left\vert\frac{n}{\sqrt[3]{n^3+1}}-1\right\vert
=\left\vert\frac{n-\sqrt[3]{n^3+1}}{\sqrt[3]{n^3+1}}\right\vert
=\frac{\sqrt[3]{n^3+1}-n}{\sqrt[3]{n^3+1}}
$$

and

$$
n^3+1<(n+1)^3\Leftrightarrow\sqrt[3]{n^3+1}<n+1\Leftrightarrow\sqrt[3]{n^3+1}-n<1.
$$

Let $\epsilon>0$. By archimedean property, there exists $N\in\N$ such that $\frac{1}{N}<\epsilon$.

Thus, $\forall n\geq N$, we have

$$
\frac{\sqrt[3]{n^3+1}}{\sqrt[3]{n^3+1}-n}
>\sqrt[3]{n^3+1}>n\geq N
$$

so that 

$$
\frac{\sqrt[3]{n^3+1}-n}{\sqrt[3]{n^3+1}}<\frac{1}{N}<\epsilon.
$$

Hence,

$$
\lim_{n\to\infty}{\frac{n}{\sqrt[3]{n^3+1}}}=1
$$
