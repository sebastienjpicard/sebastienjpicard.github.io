+++
date = '2026-10-12T11:46:27-04:00'
draft = false
katex = true
title = 'Infinitude of the Primes'
+++

By way of contradiction, we prove that there exists infinitely many primes in $ \mathbb{N} $.

<div style="margin-left: 3em;"><br>

*Proof.* &emsp; Suppose for contradiction that there exists finitely many primes $ p_1, \dots, p_n $. Let $ P = p_1 p_2 \cdots p_n + 1$. Since $ P > 1$, there exists a prime $q$ such that $ q \mid P $. However since dividing $ P $ by any $ p_i $ leaves remainder $1$, it follows that $q$ is a prime not in $p_1, \dots, p_n $, contradicting the assumption that $p_1, \dots, p_n$ contains all primes. Hence the set of primes is infinite.
<span style="float: right;">$\blacksquare$</span>
</div><br>

Note that $ p_i \mid p_1 p_2 \cdots p_n $, which implies $ P = p_1 p_2 \cdots p_n + 1$ is one more than a multiple of $ p_i $. Moreover, whether $P$ is prime is irrelevant within the context of our proof.

Our proof need not be by contradiction. Its original formulation by Euclid is direct.
