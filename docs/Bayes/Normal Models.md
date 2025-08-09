---
layout: default
title: Normal Models
nav_order: 1
math: mathjax3
parent: Bayes
---

## Normal Modeling
This page is about Bayesian models using the _normal_ (or _Gaussian_) distribution. The 1-dimensional (real) Gaussian distribution with mean $\mu$ and variance $\sigma^2$ is

\begin{equation}
f(x) = \frac{1}{\sqrt{2\pi\sigma^2}} \exp\left\\{-\frac{1}{2\sigma^2}(x - \mu)^2\right\\}.
\end{equation}

The _standard deviation_ is the square root of the variance, i.e., $\sigma$. However in Bayesian analysis we typically prefer the variance parameter as it's actually a momement of the distribution and a _scale_ parameter, so we will use $\sigma^2$ as a variable itself (instead of as a variable $\sigma$ squared).

The _n_-dimensional Gaussian distribution (or _multivariate normal_) has mean $\mu$ (now an _n_-dimensional vector) and covariance matrix $\Sigma$, an $n \times n$ symmetric positive definite matrix. The pdf is:

\begin{equation}
f(x) = (2\pi)^{-k/2}\lvert \Sigma \rvert^{-1/2}\exp\left\\{\frac{-1}{2}\left(x - \mu)^T\Sigma^{-1}(x-\mu)\right\\}.
\end{equation}

## To Do
 1. Introduction to Bayes
 1. Normal Modeling (write out normal with unknown mean, unknown std dev., both)
 1. Hierarchical modeling (write out a model here?)
 1. Page about distributions (easy to write if you want to spend time on this)
 1. Bayes as logic (from Jaynes/the talk you gave)
 1. Would be fun to do software examples
 1. List of conjugate distributions would be nice