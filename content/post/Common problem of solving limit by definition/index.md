---
title: កំហុសដែលពេញនិយម ពេលដោះស្រាយ​លីមីត​នៃស្វ៊ីត​តាមនិយមន័យ
date: 2020-06-04
math: true
diagram: true
markup: mmark
---
យើងនឹងធ្វើការបង្ហាញ និងកែលំអនូវកំហុសមួយដែលសិស្ស និស្សិត និង លោកគ្រូ អ្នកគ្រូ មួយចំនួនតែងបង្ករឡើង ពេលដោះស្រាយលីមីតនៃស្វ៊ីតតាមនិយមន័យ ។ ពិនិត្យមើល ឧទាហរណ៍ខាងក្រោម៖

ឧទាហរណ៍ 1: Prove by definition that

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

ខាងក្រោមនេះ គឺជាដំណោះស្រាយរបស់សិស្ស និស្សិត និងលោកគ្រូ អ្នកគ្រូមួយចំនួន៖

Let $\epsilon>0$, if $$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon$$ then $$\frac{1}{n^2+1}<\epsilon$$ so that $$n>\sqrt{\frac{1}{\epsilon}-1}$$

Choose $N=\left[\sqrt{\dfrac{1}{\epsilon}-1}\right]+1$ then $\forall n\geq N$, we have
$$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon$$.

Hence,

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

កំហុស​ក្នុងដំណោះស្រាយ​ខាងលើ​ គឺការកំណត់តម្លៃ $N$។ $N$ មិនអាចកំណត់បានទេ ប្រសិនបើ  $$\epsilon$$ មានតម្លៃធំខ្លាំង ។ កំហុសតូចនេះ ជាធម្មតាកើតឡើង នៅពេលដែលយើង មិនបាន​យល់​ច្បាស់​ពី​និយមន័យ ហើយ​គិត​ថា តម្លៃ $$\epsilon$$ គឺជ្រើសរើស​យក​តូចបំផុត ។ ជាការពិត យើង​អាច​ស្រាយបញ្ជាក់ ចំពោះតែ​ករណី $$\epsilon$$ តូចក៏បាន បើសិនជាយើងបានស្រាយភាពសមមូលជាមួយនឹងនិយមន័យដើម ។

យើងនឹងផ្តល់ជូននូវដំណោះស្រាយបីផ្សេងគ្នា ទាក់ទងនឹងឧទាហរណ៍ខាងលើ។

ដំណោះស្រាយ

ដំណោះស្រាយ 1: ប្រើប្រាស់និយមន័យ ចំពោះគ្រប់ $\epsilon>0$.

Given $\epsilon>0$, then

$$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon\Leftrightarrow\frac{1}{n^2+1}<\epsilon\Leftrightarrow n^2>\frac{1}{\epsilon}-1$$ 

Define

$$ N=
\begin{cases}
\left[\sqrt{\dfrac{1}{\epsilon}-1}\right]+1 & \text{ if } 0<\epsilon<1 \\
1 & \text{ if } \epsilon\geq 1
\end{cases}
$$

then $$\forall n\geq N$$, we have

$$ n^2\geq N^2>\frac{1}{\epsilon}-1 \Rightarrow
\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon$$

Hence,

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

ដំណោះស្រាយ 2: ប្រើប្រាស់តម្លៃ $\epsilon$ តូច រួចពង្រីកទៅតម្លៃ $\epsilon>0$ វិជ្ជមានទូទៅ.

Let $0<\epsilon\leq 1$, then

$$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon\Leftrightarrow\frac{1}{n^2+1}<\epsilon\Leftrightarrow n^2>\frac{1}{\epsilon}-1>0\Leftrightarrow n>\sqrt{\frac{1}{\epsilon}-1}$$

Choose $$N_\epsilon=\left[\sqrt{\dfrac{1}{\epsilon}-1}\right]+1$$ then $$\forall n\geq N_\epsilon $$, we have

$$ n>\sqrt{\frac{1}{\epsilon}-1}\Rightarrow\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<\epsilon $$

If $$\epsilon> 1$$, choose $N=N_1$ then $$\forall n\geq N$$, we have
$$\Big\vert\frac{n^2}{n^2+1}-1\Big\vert<1<\epsilon$$.

Hence,

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

ដំណោះស្រាយ 3: ប្រើប្រាស់ archimedean property.

Given $\epsilon>0$. By archimedean property, there exists $N\in\mathbb{N}$ such that $\frac{1}{N}<\epsilon$. Then for all $n\geq N$, we have

$$
\Big\vert\frac{n^2}{n^2+1}-1\Big\vert=\frac{1}{n^2+1}\leq \frac{1}{N^2+1}\leq\frac{1}{N}<\epsilon.
$$

Hence,

$$\lim_{n\to\infty}{\frac{n^2}{n^2+1}}=1$$

យើងសង្កេតឃើញថា នៅក្នុងដំណោះស្រាយទី 3 យើងមិនចាំបាច់គណនារកតម្លៃ $N$ ឡើយ។ ការ​គណនា​តម្លៃ $N$ អាច​មាន​ភាព​ស្មុគស្មាញ និង​ពិបាក​ទៅ​តាម​ប្រភេទ​នៃ​ស្វ៊ីត ។ ដូចនេះ archimedean property ជាលក្ខណៈសំខាន់មួយដែលសិស្ស និស្សិត គួរយល់ និង​ ចាំ ពេលដោះស្រាយលីមីតនៃស្វ៊ីតតាមនិយមន័យ។ Archimedean property មាន 2 និយមន័យ ដែលសមមូលគ្នាដូចខាងក្រោម៖

និយមន័យ 1: ចំពោះ​គ្រប់​ចំនួន​ពិត $x$, មាន​ចំនួន​គត់​វិជ្ជមាន $n$ ដែល $x < n$.

និយមន័យ 2: ចំពោះ​គ្រប់​ចំនួន​ពិត $a$ និង $b$ ដែល $a < b$, មានចំនួនគត់វិជ្ជមាន $n$ ដែល $b < na$.

យើង​នឹង​ដោះស្រាយ​លីមីត​នៃ​ស្វ៊ីត​តាម​និយម​ន័យ តាម​​រយៈឧទាហរណ៍​ខាងក្រោម​ ដោយ​ប្រើ​ប្រាស់ archimedean property។ អ្នកអាន គួរ​តែ​សាក​ល្បង​ដោះ​ស្រាយ​តាម​ពីរ​វិធី​ផ្សេង​ទៀត ដើម្បី​ធ្វើ​ការ​ប្រៀប​ធៀប​ និង ដើម្បីយល់​ពីប្រយោជន៍​របស់ archimedean property អោយកាន់តែច្បាស់ ។

ឧទាហរណ៍ 2: Prove by definition that

$$
\lim_{n\to\infty}{\frac{n}{\sqrt[3]{n^3+1}}}=1.
$$

ដំណោះស្រាយ: For all $n=1,2,\cdots$, we have

$$ \left\vert\frac{n}{\sqrt[3]{n^3+1}}-1\right\vert
=\left\vert\frac{n-\sqrt[3]{n^3+1}}{\sqrt[3]{n^3+1}}\right\vert
=\frac{\sqrt[3]{n^3+1}-n}{\sqrt[3]{n^3+1}}$$

and

$$ n^3+1 < (n+1)^3 \Leftrightarrow \sqrt[3]{n^3+1}-n < 1 .$$

Let $\epsilon>0$. By archimedean property, there exists $N\in\mathbb{N}$ such that $\frac{1}{N}<\epsilon$.

Thus, $\forall n\geq N$, we have

$$
\frac{\sqrt[3]{n^3+1}}{\sqrt[3]{n^3+1}-n} > \sqrt[3]{n^3+1} > n\geq N
$$

so that 

$$
\frac{\sqrt[3]{n^3+1}-n}{\sqrt[3]{n^3+1}} < \frac{1}{N} < \epsilon.
$$

Hence,

$$
\lim_{n\to\infty}{\frac{n}{\sqrt[3]{n^3+1}}}=1
$$

គួរកត់សម្គាល់ផងដែរថា កំហុសនេះ ក៏​កើត​មានឡើង​ផង​ដែរ​ នៅ​ក្នុង​ដំណោះ​ស្រាយលីមីតនៃ​អនុគមន៍​តាម​និយម​ន័យ​ $$\epsilon-\delta$$ នៅ​ពេល​ជ្រើស​រើស​យកតម្លៃ $\delta$ ហើយការកែតម្រូវ​មាន​ភាព​ស្រដៀង​គ្នា ដូច​ទៅ​នឹងលីមីត​ស្វ៊ីត​ខាងលើ៕​

