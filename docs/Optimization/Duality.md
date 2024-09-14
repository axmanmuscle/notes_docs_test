---
layout: default
title: Conjugates and Duality
nav_order: 2
math: mathjax3
parent: Optimization
---

## Introduction
Duality is an important concept in both functional analysis and convex optimization. Let's start with some definitions. See Bauschke and Combettes for more.

### Definition
Let $f: \mathcal{H} \to [-\infty, +\infty]$. The _conjugate_ (or _Fenchel conjugate_, or _Legendre transform_, or _Legendre-Fenchel transform_) for $f$ is
$$f^* : \mathcal{H} \to [-\infty, +\infty] : u \to \sup_{x \in \mathcal{H}} \langle x, u \rangle - f(x).$$

### Examples
The conjugate of $f = \lVert \, \cdot \, \rVert$ is given by
$$f^*(y) = \begin{cases} 0 & \lVert y \rVert_* \leq 1 \\ \infty & \text{otherwise} \end{cases},$$
the indicator function of the dual norm unit ball.