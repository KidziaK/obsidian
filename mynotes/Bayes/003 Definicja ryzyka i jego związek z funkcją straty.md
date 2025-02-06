#### Funkcja straty i ryzyko
Funkcję $l(z, a)$ będziemy nazywać funkcją straty. Będzie nas interesować scenariusz, gdzie na podstawie zmiennej losowej $Z$ będziemy chcieli podjąć akcję ze zbioru $\mathscr{A}$ która w jakimś sensie minimalizuje nasza stratę. Zwykle będziemy chcieli minimalizować średnią stratę, czyli tak zwane ryzyko $r(a) = \mathbb{E} l(Z, a).$ Innymi słowy staramy się rozwiązać problem optymalizacyjny $$ \underset{a \in \mathscr{A}}{\mathrm{argmin}} \ r(a)$$
#### Reguły decyzyjne
Rozważmy następujący model. Nasze dane składają się z par $X, Y.$ Będzie nas interesowało przewidywanie wartości $Y$ przy danym $X.$ Wprowadzamy tak zwaną regułę decyzyjną $\delta(X)$ czyli w zasadzie estymację $Y$ przy danym $X$ i wybieramy funkcję straty odpowiadającą naszemu problemowi $$ l(Y, \delta(X))$$ Dla tak zdefiniowanej straty będziemy chcieli minimalizować ryzyko $$ R(\delta) = \mathbb{E} l(Y, \delta(X)) $$Regułę $\delta^*$ która minimalizuję powyższe ryzyko nazywamy **regułą Bayesowską**. 

#### Ryzyko aposteriori
Aby określić optymalną regułę decyzyjną wystarczy obliczyć tak zwane ryzyko aposteriori przy ustalonej obserwacji $x$ dla różnych decyzji $a.$ Ryzyko aposteriori wyraża się wzorem $$r(a|x) = \mathbb{E}(l(Y, a) | X=x)$$
#### Gra statystyczna i ryzyko Bayesowskie
