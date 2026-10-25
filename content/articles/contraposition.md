+++
date = '2026-10-14T21:19:32-04:00'
draft = false
katex = true
title = 'Contraposition'
+++

Recall that the **CONTRAPOSITIVE** of an implication is as follows, $P \Rightarrow Q \equiv \neg Q \Rightarrow \neg P$. We prove by way of contraposition that if $n^2$ is even, then $n$ is even also. 

<div style="margin-left: 3em;"><br>

*Proof.* &emsp; Suppose $n \in \mathbb{Z}$ is odd, that is, $ n = 2k + 1 $ for some $ k \in \mathbb{Z} $. We thus have $$ n^2 = (2k + 1)^2 = 2(2k^2 + 2k) + 1.$$ Since $n^2$ is of the form $2m + 1,\ m \in \mathbb{Z}$, it follows $n^2$ is odd. Since the contrapositive holds, so does our original claim. Hence if $n^2$ is even, then $n$ is even.
<span style="float: right;">$\blacksquare$</span>
</div><br>

Notice that the converse claim need not be proven by contraposition, and can be proven directly with some algebraic manipulation. As an exercise, attempt to prove the claim directly and observe why it is impossible to do so.

Prove that if $c > \frac{49}{8}$ then $y = 2x^2 + 7x + c$ has no real roots. Proceed by contraposition.
<div style="margin-left: 3em;"><br>

*Proof.* &emsp; We show that if $y = 2x^2 + 7x + c$ has real roots, then $c \le \frac{49}{8}$. A quadratic polynomial $ ax^2 + bx + c = 0 $ has real roots if and only if $ b^2 - 4ac \ge 0 $. Let $a = 2$ and $b = 7 $. We obtain $7^2 - 4(2c) = 49 - 8c \ge 0$, thus $ c \le \frac{49}{8} $. Since the contrapositive holds, so does our original claim. Hence if $c > \frac{49}{8}$, then $y = 2x^2 + 7x + c$ has no real roots.
<span style="float: right;">$\blacksquare$</span>
</div><br>

