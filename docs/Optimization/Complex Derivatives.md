---
layout: default
title: Complex Derivatives
nav_order: 3
math: mathjax3
parent: optimization
---

## Introduction
As we discussed in [Linear] (need to learn how to make links to other posts), vector spaces with a complex scalar field present a unique challenge to optimization. Compelx numbers are common parameters in engineering and signal processing applications, such as communications, MRI/CT/medical image reconstruction, SONAR location finding, etc. Since optimization methods most frequently make use of derivatives, a question of how to take a derivative of a function of a complex number comes up often.

## Complex Numbers
Define $i$ such that $i^2 = -1$. A complex number can be written as
$$z = a + bi$$
with $a, b \in \mathbb{R}$. Even though $a, b$ are both real, we'll call $a$ the _real_ part of $z$ and $b$ the _imaginary_ part. Formally, define $Re: \mathbb{Z} \to \mathbb{R}$ as $Re(a + bi) = a$ and $Im: \mathbb{Z} \to \mathbb{R}$ as $Im(a + bi) = b$. The _magnitude_ of $z$ in this case is defined as
$$\lvert{z\rvert} = \sqrt{a^2 + b^2}. $$
This is the same as the two norm if we were to stack $a, b$ on top of each other and imagine it as a vector in $\mathbb{R}^2$. 

Another common way to write complex numbers is as
$$z = k e^{i\theta}$$
where we'll denote $k$ as the _magnitude_ of $z$ and $\theta$ as the _argument_. 

## Complex Derivatives
Let's write the complex numbers in a slightly more esoteric way:
$$z(v_r, v_i) = v_r + v_ii$$