---
title: "Monotone Convergence Theorem"
date: 2026-08-06T15:44:45-04:00
draft: false
latex: true
---

Let $a:\mathbb{N} \to \mathbb{R}\ \{a_n\}$ be a sequence of real numbers. If $\{a_n\}$ is **MONOTONICALLY INCREASING**, that is for all $n \in \mathbb{N}, \ a_{n+1} \ge a_n$, and **BOUNDED ABOVE**, that is for all $n,\ a_n \le B$ for some $B \in \mathbb{R}$, then $\{a_n\}$ converges to a finite value as $n \to \infty$.  Likewise if $\{a_n\}$ is **MONOTONICALLY DECREASING**, that is for all $n \in \mathbb{N}, \ a_{n+1} \le a_n$, and **BOUNDED BELOW**, that is for all $n, \ a_n \ge b$ for some $b \in \mathbb{R}$, then $\{a_n\}$ converges to a finite value as $n \to \infty$.

We prove each case separately. For both cases, we want to show that, by **DEFINITION OF CONVERGENCE**,
 
$$\exists L \in \mathbb{R} \text{ s.t. } \forall \varepsilon > 0, \ \exists N \in \mathbb{N} \text{ s.t. } \forall n \geq N, \ |a_n - L| < \varepsilon.$$

The definition essentially states that a sequence $\{a_n\}$ is convergent if there exists a point $L$ such that beyond some index $N$, every term of the sequence lies within an arbitrary distance $\varepsilon$ of $L$ and never escapes that bound.

<div style="margin-left: 3em;"><br>

*Proof.* &emsp; Since $\{a_n\}$ is nonempty and bounded above, by the **LEAST-UPPER-BOUND PROPERTY** of $\mathbb{R}$, there exists a least upper bound $L$ of $\{a_n\},\ L = \sup \{a_n\}$. Let $\varepsilon > 0$. Since $L$ is the least upper bound of $\{a_n\},\ L - \varepsilon$ is not an upper bound, hence $\exists N \in \mathbb{N} \text{ s.t. } a_N > L - \varepsilon$.

Since $\{a_n\}$ is monotonically increasing, $\forall n \ge N,\ a_n \ge a_N > L - \varepsilon$. Moreover since $L = \sup\{a_n\}$ is an upper bound of $\{a_n\}, \ \forall n \ge N,\ a_n \leq L < L + \varepsilon$.

Combining the above, $\forall n \ge  N, \ L - \varepsilon < a_n < L + \varepsilon\ \implies \forall n \ge N, \ |a_n - L| < \varepsilon$.  Since $\varepsilon > 0$ was arbitrary, by definition of convergence, $\{a_n\}$ converges to $L$.
<span style="float: right;">$\blacksquare$</span>
</div><br>

The decreasing case is effectively the mirror image of the increasing case---making use of the greatest lower bound in place of the least upper bound---and is left as an exercise for the reader.

Note that in our proof, we make use of the fact that if for all $n \in \mathbb{N},\ a_{n+1} \ge a_n$, then for all $n \ge N,\ a_n \ge a_N$. While trivial, proving it makes for a good exercise. Proceed by induction on $n$.

<div style="margin-left: 3em;"> <br>

*Proof.* &emsp; For the base case $n=N$, it immediately follows that $a_n \ge a_N$. For the inductive step, suppose $a_k \ge a_N$ for some $k \ge N$. Since $a_{k+1} \ge a_k$, it follows that $a_{k+1} \ge a_k \ge a_N$, therefore $a_{k+1} \ge a_N$, as needed. Hence for all $n \ge N, \ a_n \ge a_N$.
<span style="float: right;">$\blacksquare$</span>
</div> <br>

<!-- Let's go through some worked examples. -->