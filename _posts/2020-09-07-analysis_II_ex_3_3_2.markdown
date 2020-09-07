Analysis II, Exercise 3.3.2

Theorem 3.3.1

Proposition 3.3.3.

This proposition has the concise, appealing conclusion, that you may exchange the limits if the sequence of funcitons converges uniformly. It's worth a while, though, to think carefully about the proof.

Note first that using Theorem 3.3.1 is easy (equivalent?)

$$ \lim_{n \rightarrow \infty} \lim_{x \rightarrow x_0} f_n(x) = \lim_{x \rightarrow x_0} \lim_{n \rightarrow \infty} f_n(x) $$

We will dissect it piece by piece. First, $\lim_{x \rightarrow x_0} f_n(x)$, with a fixed n, is the functional limit of the function $$f_n$$, thus the limit is a real number. The limit exist, and in fact it is $$f_n(x_0)$$ because by assumption $f_n$ is continuous.

Thus the left hand side boils down to $\lim_{n \rightarrow \infty} (f_n(x_0))$, where $(f_n(x_0))$ is a sequence of real numbers. Does it converge? Sure, because by assumption $(f_n)$ converges uniformly to $f$. Thus the left hand side is well-defined, and evaluates to $f(x_0)$.

Let us now consider the right hand side. For all $x \in X$, we have $\lim_{n \rightarrow \infty} f_n(x) = f(x)$ by the assumpiton that $(f_n)$ is uniformly convergent. But we don't know (yet) whether $f$ is continuous, thus whether the limit $\lim_{x \rightarrow x_0} \lim_{n \rightarrow \infty} f_n(x) = \lim_{x \rightarrow x_0} f(x)$ exists is not clear. (e.g. Dirichlet's function $f:[0,1] \mapsto \{ 0, 1 \}$, where $f(x) = 1$ for all rational x and $f(x) = 0$ elsewhere, doens't have the limit at all $x \in [0,1]$).

Thus our task is to prove that the limit $\lim_{x \rightarrow x_0} f(x)$ exists, and it is in fact equal to the left hand side, $f(x_0)$.

**Proof.** We will


$\square$. 