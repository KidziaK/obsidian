#### Dostateczność a warunkowa niezależność
W statystyce Bayesowskiej warunkowa niezależność jest w zasadzie równoważna dostateczności (z dokładnością do pewnych teorio miarowych niuansów).

*Twierdzenie*
Następujące warunki są równoważne:
1) $X$ i $\nu$ są warunkowo niezależne pod warunkiem $T(X)$
2) Zachodzi własność faktoryzacji $p_{\theta}(x) = g_{\theta}(T(x))h(x)$ 

#### Wykładnicza rodzina rozkładów
Powiemy, że rozkład należy do wykładniczej rodziny rozkładów jeśli ma postać $$p_{\theta}(x) = \exp\left(\sum_{j=1}^{k}T_j(x)g_j(\theta) + g_0(\theta)\right)h(x)$$
#### Sprzężone rodziny rozkładów 
Rozkład apriori $\pi(\theta)$ nazwiemy sprzężonym do $p_{\theta}(x)$ jeżeli rozkład aposteriori ma tę samą postać i inne parametry co $\pi(\theta)$ dla dowolnego $n.$ Dla wykładniczej rodziny rozkładów, rozkład apriori postaci $$\pi(\theta) = c(t_0, n_0)\exp\left( \sum_{j=1}^{k} t_{0j}g_j(\theta) + n_0 g_0(\theta) \right) $$ jest sprzężony do $p_{\theta}(x).$

#### Rozkłady Jeffreysa
Rozkład $\pi(\theta) \sim \sqrt{I(\theta)} = \sqrt{\mathbb{E}_{\theta} \left(\frac{d}{d\theta}log(p_{\theta}(X)) \right)^2}$ będziemy nazywać rozkładem Jeffreysa.