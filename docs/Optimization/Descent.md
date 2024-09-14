---
layout: default
title: Descent
nav_order: 1
math: mathjax3
parent: Optimization
---

## Introduction
The most intuitive optimization algorithm (and often the first taught, in an introductory calculus course) is a _descent method_. The concept makes sense: we have a function $f$ which we want to minimize. We're at a point $x$ with function value $f(x)$. Let's choose a direction $\mathbf{p}$ such that $f(x + \mathbf{p}) < f(x)$! We want to make the function value decrease, so let's choose the direction that does that! Groundbreaking. 

In its simplest form, our problem is
$$
\begin{equation}
\underset{x \in \mathcal{H}}{\text{minimize}}\; f(x)
\label{eq:primal}
\end{equation}
$$
where $\mathcal{H}$ is a Hilbert space and $f$ is a continuous function $f: \mathcal{H} \to \mathcal{H}$. Our algorithm is, given some point $x_k$, choose point 

$$
\begin{equation}
x_{k+1} = x_k + \mathbf{p}
\label{eq:descent}
\end{equation}
$$

such that $f(x_{k+1}) \leq f(x_k)$. Note here that $p \in \mathcal{H}$ as well, so if $x_k$ is a vector than $\mathbf{p}$ is as well. We've put no restrictions or assumptions on how $f$ behaves (besides continuity), whether it actually _possesses a minimizer at all_, etc. As we place more assumptions on $f$ we can get a better handle on what a good choice of descent direction is.

Often we'll associate with a descent method a _step size_ in that direction, turning \eqref{eq:descent} into

$$
\begin{equation}
x_{k+1} = x_k + \alpha\mathbf{p}
\end{equation}
$$
where $\alpha$ is the step size. There are different heuristics or searches for choosing a step size based on other characteristics of the problem and the function $f$.

## Gradient Descent
This is the most popular form of descent algorithm. We'll assume that $f$ is _continuously differentiable_, so we have $f'(x)$ and it's well defined. 