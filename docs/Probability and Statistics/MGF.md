---
layout: default
title: Moment Generating Functions
nav_order: 3
math: mathjax3
parent: Prob&Stats
---

## Moment Generating Functions
A useful concept for certain probability problems (e.g. distribution of _sums_ of random variables) is the _moment generating function_.

#### Definition: Moments
A _moment_ of a random variable $X$ describes some behavior about the graph of the density function.

#### Definition: Moment Generating Function
Let $X$ be a random variable with pdf $f$. The moment generating function is given by

\begin{equation}
m(t) = \mathcal{E}\left[e^{tX}\right].
\end{equation}

The $n^{\text{th}}$ moment of $X$ is given by

\begin{equation}
\frac{\text{d}}{\text{dt}} m(t)\,\rvert_{t = 0}.
\end{equation}
