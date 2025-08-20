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
f(x) = (2\pi)^{-k/2}\vert \Sigma \vert^{-1/2}\exp\left\\{\frac{-1}{2}\left(x - \mu\right)^T\Sigma^{-1}\left(x-\mu\right)\right\\}.
\end{equation}

The inverse of the covariance matrix is called the _precision matrix_ $Q = \Sigma^{-1}$. 

There are usually one of three goals with a Normal model:
  1. Estimate the mean with a known variance
  1. Estimate the variance with a known mean
  1. Estimate both the mean and the variance jointly

As is usually the case with Bayesian analysis, we will treat these parameters as _random variables_ and attempt to estimate their _distributions_.

### Unknown Mean, Known Variance
For this first model, the conjugate prior choice for the mean (or _location parameter_) is also a Normal distribution. So here is the set up. Suppose our likelihood is
\begin{equation}
\begin{aligned}
x_i \, \vert \, \mu &\sym \mathcal{N}\left(\mu, \sigma^2) \\
\mu &\sym \mathcal{N}\left(\mu_p, \sigma_p^2).
\end{equation}
In this model, $\mu_p$ and $\sigma_p$ are specified hyperparameters (not parameters being estimated).

## To Do
 1. Introduction to Bayes
 1. Normal Modeling (write out normal with unknown mean, unknown std dev., both)
 1. Hierarchical modeling (write out a model here?)
 1. Page about distributions (easy to write if you want to spend time on this)
 1. Bayes as logic (from Jaynes/the talk you gave)
 1. Would be fun to do software examples
 1. List of conjugate distributions would be nice


I think it would be nice to do like, normal-normal model for mean, then show what it looks like as you add data. Then also python code to do it

Then MCMC? Like what if the data is normal and we have a tight prior on the mean (uniform?) what happens then?