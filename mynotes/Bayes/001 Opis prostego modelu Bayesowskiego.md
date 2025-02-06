#### Model Bayesowski i rozkład *a priori*
Niech $X$ będzie obserwowaną zmienną losową z rozkładu $P_{\theta},$ a $\theta$ będzie realizacją innej zmiennej losowej $\nu$ z rozkładu $\Pi.$ Rozkład $\Pi$ będzie nazywać rozkładem *a priori.* Rozkład a priori możemy interpretować jako nasza wiedza o nieznanym parametrze $\theta$ przed zaobserwowaniem danych. Forma rozkładu a priori może być *informatywna* czyli wynikać na przykład z wyników wcześniejszych eksperymentów, albo wiedzy eksperckiej. Albo *nieinformatywna* gdzie narzucony rozkład ma pewne użyteczne własności statystyczne, ale jego struktura niekoniecznie wynika z analizy wcześniejszych danych.

#### Rozkład *a posteriori*
W praktyce będzie chcieli powiedzieć coś o nieznanym parametrze $\theta$ używając nie tylko rozkładu a priori, ale również zaobserwowanych danych. W tym celu wprowadzamy pojęcie rozkładu *a posteriori* $\pi(\theta | x) = \frac{p(x|\theta)\pi(\theta)}{p(x)}$  (ze wzoru Bayesa).

#### Warunkowa niezależność
Niech $X, Y, Z$ będą zmiennymi losowymi. Powiemy, że $X \perp Y | Z$ ($X$ jest warunkowo niezależna od $Y$ pod warunkiem $Z$) jeżeli jest spełniony jeden z dwóch równoważnych warunków:

1) $p(x,y|z) = p(x|z)p(y|z)$
2) $p(x|y,z)=p(x|z)$ i  $p(y|x,z)=p(y|z)$

W modelu Bayesowskim będziemy zakładać, że obserwacje są warunkowo niezależne pod warunkiem parametru.

#### Rozkład predykcyjny
Często będzie nas interesowała predykcja następnego, jeszcze niezaobserwowanego $X_n$ z rozkładu $p_{\theta}.$ W tym celu będziemy używać rozkładu predykcyjnego $$\begin{align*} p(x_n|x_{n-1}\dots x_{1}) &= \int_{\Theta} p(x_n|\theta,x_{n-1},\dots x_1)p(\theta|x_{n-1},\dots x_1)d\theta \\ &\stackrel{\text{warunkowa niezależność}}{=} \int_{\Theta} p(x_n|\theta) p(\theta|x_{n-1},\dots x_1)d\theta \end{align*}$$