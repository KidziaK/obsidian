#### Explicit representation (parametric)
$$f: U \rightarrow M$$
Where $U$ is an open subset of $\mathbb{R}^n$ or $\mathbb{E}^n$ and $M$ is a differential manifold.

**Examples**
- curve $\gamma(t) = (x(t), y(t), z(t))$
- surface $S(u, v) = (x(u, v),\ y(u, v),\ z(u, v))^T$
- volume $V(u, v, w) = (x(u, v, w),\ y(u, v, w)\ z(u, v, w))^T$
**Notes**
- non-unique representation of a manifold $\gamma(t)$ is the same curve as $\gamma(f(t))$ for any bijection $f.$
#### Implicit representation
Manifold defined as a set of points satisfying given equation $M = \{x \in \mathbb{R}^n | P(x) = 0 \}.$ 

**Examples**
- sphere $x^2 + y^2 + z^2 - 1 = 0$
- line $\{A_x x + A_y y + A_z z + A_s = 0\} \cap \{B_x x + B_y y + B_z z + B_s = 0\}$  
### Benefits and drawbacks of representations

|                | point belongs to manifold | generating points | calculating normals |
| -------------- | ------------------------- | ----------------- | ------------------- |
| **parametric** | ❌                         | $\checkmark$      | $\checkmark$        |
| **implicit**   | $\checkmark$              | ❌                 | $\checkmark$        |
