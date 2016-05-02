---
layout: post
title: Generalised Distributive Law
---

A very short entry on a little theorem I stumbled upon the other day. Let $R$ be a ring, and $X$ and $Y$ be finite indexing sets for some arbitrary map $a : X \times Y \to R$. Then

$$
  \prod_{x \in X} \sum_{y \in Y} a(x,y)
  \equiv
  \sum_{f \in \text{Maps}(X, Y)} \prod_{x \in X} a(x, f(x))
$$

Basically this allows you to swap the order of the sum and product operators. The proof is rather intuitive:

$$
\begin{align}
\prod_{x \in X} \sum_{y \in Y} a(x,y) &= \prod_{x \in X} a(x, y_1) + \dots + a(x, y_n)\\
&= \overbrace{(a(x_1, y_1) + \dots + a(x_1, y_n))}^{x1} \dots \overbrace{(a(x_m, y_1) + \dots + a(x_m, y_n))}^{x_n}
\end{align}
$$

When expanding this product you "pick a term" in each bracket. This can be expressed as a map from $X$ to $Y$: bracket is identified by an element in $X$, and each term in a bracket is identified by an element in $Y$. So it is only natural that you would sum over all possible maps. Voila!

<br/>

*PS: feel free to suggest a better title*
