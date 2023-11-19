- When the question has "if and only if " statement that means it implies both ways, so we have to prove it in both directions.
- Whenever in the induction if terms are connected via their previous terms, we use strong induction instead of just proving1, n n+1.
-  **(Young Inequality)** Prove that for $p ∈ (1,∞)$, we have $xy ≤ 1$
 $px^p + 1 qy^q$  for  $x, y ∈ R+ := {x ∈ R : x ≥ 0}$, where $q = p/p−1$ is the Holder conjugate of $p$ determined by $1/p + 1/q = 1$
 Can be done using “log’s concavity” as $log((x^p)/p + (y^q)/q) ≥ 1/plog(x^p) + 1/qlog(y^q)=logx + logy$
- ![[Pasted image 20230918115136.png]]
- To show that there exists a rational number r such that $x < r^2 < y$, we can use proof by contradiction. 
- Suppose that there does not exist such a rational number r. Then, for any rational number $r$, either $r^2 < x$ or $r^2 > y$.
- Let A be the set of all rational numbers r such that $r^2 < x$, and let B be the set of all rational numbers r such that $r^2 > y$. Since $x < y$, we have that A and B are non-empty. 
- By the completeness axiom of the real numbers, there exists a least upper bound for A, denoted by $a$, and a greatest lower bound for B, denoted by $b$. Since a is the least upper bound for A, there exists a rational number $r1$ such that $a - 1/n < r1 < a$ for any positive integer $n$. 
- Similarly, since $b$ is the greatest lower bound for B, there exists a rational number $r2$ such that $b < r2 < b + 1/n$ for any positive integer n. Then, we have that $r1^2 < x < y < r2^2$, which implies that $(r1^2 + r2^2)/2 < y$ and $(r1^2 + r2^2)/2 > x$. 
- However, $(r1^2 + r2^2)/2$ is a rational number between x and y, which contradicts our assumption that there does not exist a rational number r such that $x < r^2 < y$. 
- Therefore, there exists a rational number r such that $x < r^2 < y$.