---
layout: default
title: Fourier Theory
nav_order: 3
math: mathjax3
parent: Signal Processing
---

## Fourier Theory
One central mathematical tool to signal processing is the _Fourier transform_. 

## To Do
 1. Intro/history? Low prio
 2. Defn
 3. Theorems (shift, slice, ?)
 4. Interpretations

## Definition
Let $f$ be a (cont? diffable? complex? real?) function. The _Fourier transform_ of $f$ is

\begin{equation}
\mathcal{F}\left\\{f\right\\}(k) = \hat{f}(k) = \int_{-\infty}^{\infty}f(x) \exp\left\\{-i2\pi kx\right\\}\mathrm{d}x,
\end{equation}

with the corresponding _inverse Fourier transform_:

\begin{equation}
f(x) = \int_{-\infty}^{\infty}\hat{f}(k) \exp\left\\{i2\pi kx\right\\}\mathrm{d}k.
\end{equation}

## Interpretations
One useful thing about these integral transforms, both this and the Laplace transform, is their effect on differential equations. Jaynes talks about this in his theory of probability book (which is excellent).