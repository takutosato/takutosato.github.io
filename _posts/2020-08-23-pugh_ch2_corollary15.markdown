---
layout: post
title:  "PUGH. Chapter 2, Corollary 15"
categories: Math
tags: [Pugh, Topology]
usemathjax: true
---

PUGH. Corollary 15, Chapter 2

$$\pi$$

_Let $$N$$ be an open subset of the metric space $$M$$. Then $$U$$ is open in $$N$$ if and only if $$U$$ is open in $$M$$ also._

($$\Rightarrow$$) Suppose $$U$$ is open in $$N$$, and let $$p \in U$$. We wish to show that there exists an open ball in $$M$$ around $$p$$ that is a subset of $$U$$.

 There exists an open ball in $$N$$ centered at $$p$$ of radius $$r_1$$ that rests fully inside $$N$$; that is, there exists $$B_N(p,r_1) \subset U$$. The question then is, once we let the points in $$M$$ in this ball---that is, when we consider the ball of the same radius $$r$$ \textit{in $$M$$}, $$B_M(p,r_1) \subset U$$---does the ball remain a subset of $$U$$?
 
 In the general case, when $$N$$ is not necessarily an open subset of $$M$$, this is not the case. For instance, take $$M = \real$$, $$N = \mathbb{Q}$$, and $$U = (0,1) \cap \mathbb{Q}$$. Then $$B_{\Q}(0.5, 0.1)$$ is a subset of $$U$$, but $$B_{\real}(0.5, 0.1)$$ is not, because we let in the real numbers near 0.5.
 
 However, since we have here that $$N$$ is an open subset of $$M$$, there exists another ball of radius $$r_2$$ centered at $$p$$ in the metric space $$M$$ such that $$B_M(p,r_2) \subset N$$. Let $$r = \min(r_1, r_2)$$, and consider $$B_M(p,r)$$. Let $$y \in B_M(p,r)$$. $$r \leq r_2$$ ensures that $$y \in N$$. Further, $$r \leq r_1$$ means that $$y \in U$$ also. Thus we have found an interior of $$U$$ at point $$p$$ in M, $$B_M(p,r) \subset U$$, thus $$U$$ is open in $$M$$.
 
 ($$\Leftarrow$$) Now suppose $$U$$ is open in $$M$$. For each $$p \in U$$, there exists a ball in $$M$$, $$B_M(p,r) \subset U$$. Further, since $$N$$ is open in $$M$$, there exists another ball $$B_M(p,r') \subset N$$. Now take the intersection of the two balls, which is also open and therefore has an open ball $$B_M(p,\epsilon)$$ centered at $$p$$ that is an interior of the intersection. All $$y \in B_M(p,\epsilon)$$ is an element of $$U$$, and also of $$N$$, thus it follows that $$B_M(p,\epsilon) \subset N$$. Since $$p$$ is an arbitrary element of $$U$$, it follows that $$U$$ is open in $$N$$, as desired.