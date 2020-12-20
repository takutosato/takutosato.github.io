---
tags: ["analysis", "problem", "SS"]
title: The behavior of an integrable function at large x
---

Integrability of a function $f$ on $\mathbb{R}$ suggests that $f$ is not too large, both in the sense that

1. $f$ is nearly bounded
2. $f$ is nearly zero at large $\vert x \vert$.

$f$ integrable implies $f$ is bounded a.e.. (Proof: Suppose on the contrary that $f$ is unbounded on a set of positive measure. Let $E$ denote this set, and define $g_N(x) = N\chi_E$. Then $f \geq g_N$ for all $N$. But $\int g_N = N m(E)$, which grows unbounded with $N$.)

On the other hand, $f$ integrable does not imply that $f$ approach $0$ as $x \rightarrow 0$. Conisder, for example the function

$$ f = \sum_{n} n \chi_{[n, 1/n^3]}, $$

which looks like towers of increasing height and decreasing width placed at integers. The integral of $f$ is $\sum_{n} (1/n^2) = \pi^2/6$ (the sum of the series $\sum_{n=1} 1/n^q$ for $q > 1$ is given by the Riemann-Zeta function $\zeta$, and $\zeta(2) = \pi^2/6$.) and therefore $f$ is integrable, despite the fact that $\limsup f(x) = \infty$ (lim rather than limsup is fine too here, because we are saying that neither lim or limsup is finite. If one is infinite the other must also be infinite). We could even make this continuous by adding buttresses of width $1/n^3$ on either side of the tower, which contributes $1/n^2$ to each term of the integral.

Once we add the extra condition that $f$ is uniformly continuous, however, then $f$ must approach $0$ at large $x$.

__Proposition__. If $f:\mathbb{R} \rightarrow \mathbb{R}$ is integrable and uniformly continuous then $\lim_{\vert x \vert \rightarrow \infty} f(x) = 0$.

_Proof_. Suppose on the contrary that there exists $\epsilon > 0$ such that for all $N$ there exists $x > N$ such that $\vert f(x) \vert > \epsilon$.  Since $f$ is uniformly continuous, we may choose $\delta > 0$ such that $\vert x - x_0 \vert  < \delta$ implies $\vert f(x) - f(x_0) \vert < \epsilon/2$. Let $N_0 = 1$. Then there exists $x_0 > N_0$ such that $f(x_0) > \epsilon$. Since $f$ is uniformly continuous, all $x$ within the $\delta$-ball of $x_0$ satisfies $f(x) > \epsilon/2$, thus $(\epsilon/2)\chi_{B_{\delta}(x_0)}  \leq f$, where $\chi_{B_{\delta}}$ is the characteristic function on the $\delta$-ball around $x_0$. Letting $N_1 = x_0$, we may choose $x_1 \geq N_1$ such that $\vert f(x) \vert > \epsilon$. By the same argument, we have $(\epsilon/2) \big ( \chi_{B_{\delta}(x_0)} + \chi_{B_{\delta}(x_1)} \big ) \leq f$. We may repeat the procedure $N$ times and obtain

$$ \sum_{n=1}^N (\epsilon/2) \chi_{B_{\delta}(x_1)} \leq f, $$

and therefore $\int \sum_{n=1}^N \chi_{B_{\delta}(x_1)} \leq \int f$. But,

$$ \int \sum_{n=1}^N \chi_{B_{\delta}(x_1)} = \sum_{n=1}^N (\epsilon/2) (2\delta) = N (\epsilon * delta), $$

which grows unbounded with $N$, contradicting our assumption that $\int f$ is integrable. $\square$ 


(Adopted from Stein and Shakarchi, Chapter 2 Exercise 6.)