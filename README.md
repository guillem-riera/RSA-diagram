# RSA-diagram
RSA Diagram using mermaid. For learning purposes.

```mermaid
graph TD
	A[Start]
	B[Select two prime numbers p and q]
	C[Compute n = p*q and φ(n) = (p-1)*(q-1)]
	D[Choose an integer e such that 1 < e < φ(n) and gcd(e, φ(n)) = 1]
	E[Compute d to satisfy the congruence relation d*e ≡ 1 (mod φ(n))]
	F[Output: Public Key (n, e) and Private Key (n, d)]
	G[End]
	A --> B
	B --> C
	C --> D
	D --> E
	E --> F
	F --> G
```