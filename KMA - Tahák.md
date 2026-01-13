
# Tahák

> [!note] Kořeny kvadratické rovnice:
$$
x_{1,2} = \frac{-b\pm\sqrt{b^2-4ac}}{2a}
$$

Determinant 2x2:
det=ad−bc

Determinant 3x3:
det=aei+bfg+cdh−(ceg+bdi+afh)

## HLR
### Charakteristická rovnice:
1. Převedeme všechny členy na levou stranu 
2. členy $a_n$ nahradíme za $x^{k-n}$
3. Vytkneme $x^n$
4. Vyřešíme rovnici (najdeme kořeny)

> [!note] Kořen $r$ násobnosti $m$ vygeneruje $m$ lineárně nezávislých řešení: 
$$
\{r^n\}^\infty_{n=0}, \{nr^n\}^\infty_{n=0}, ..., \{n^{m-1}r^n\}^\infty_{n=0}
$$

### Obecné řešení:
$$
a_n = r_1^n(K_1^{(1)} +K_2^{(1)}n+...K_{m_1}^{(1)}n^{m_1-1}) +
...+
r_l^n(K_1^{(l)} +K_2^{(l)}n+...K_{m_l}^{(l)}n^{m_l-1})
$$
kde:
- $K_1^{(1)}, ..., K_{m_l}^{(l)}$ jsou libovolné konstanty (celkem $k$ konstant)

$$
F_n​=Ar_1^n​+Br_2^n​
$$

### Partikulární řešení:
Určíme konstanty z počátečních podmínek.
1. Dosadíme počáteční podmínky.
2. Vyřešíme N rovnic o n neznámých.

## Soustava rovnic

1. Sestavíme matici.
### Vlastní čísla:

$det(A-\lambda I)$

1. Odečteme $\lambda$ na diagonále.
2. Spočítáme determinant.
3. Najdeme kořeny -> vlastní vektory.
###  Vlastní vektory:
$(A - \lambda I)\mathbf{v} = \mathbf{0}$
5. Dosadíme do rovnice postupně všechny kořeny -> vlastní čísla.

Za $x$ dosadíme 1 a $y$ dopočítáme ->vlastní vektor

### Obecné řešení:
$$
x_n = c_1 \lambda_1^n v_1 + c_2 \lambda_2^n v_2
$$

## NHLR

Zkušební řešení:

| $p_n$            | $t_n$                                                     |
| ---------------- | --------------------------------------------------------- |
| K (konstanta)    | A (konstanta)                                             |
| $n^t, t\in N$    | $A_0 + A_1n+...+A_tn^t$ - polynom stupně t, A - konstanta |
| $r^n,r\in R$     | $Ar^n$                                                    |
| $r^n*n>t,t\in R$ | $r^n(A_0 + A_1n+...+A_tn^t)$                              |
| $cos(\alpha n)$  | $A cos(\alpha n) + B \sin/(\alpha n)$                     |
| $sin(\beta n)$   | $A cos(\beta n) + B \sin/(\beta n)$                       |

1. Spočítáme homogenní řešení.
2. Zkušební řešení hledáme ve tvaru pravé strany. 
    - Pokud zkušební řešení koliduje přezásobíme ho $n$.
    - Pokud kořen více násobný, pře násobíme zkušební řešení $n$. 
3. Zkušební řešení dosadíme do rekurentního vztahu za členy $a_n$...
4. Získáme koeficienty A a B...
5. Máme partikulární řešení.

> [!tip] Obecné řešení NHLR je tvaru:
$$
a_n = a_n^{(h)} + a_n^{(p)}
$$

6. Sestavíme obecné řešení.
7. Dosadíme počáteční podmínky.
## Grafy

Matice sousednosti:
- vrcholy x vrcholy
- 1 tam kde je hrana

Matice incidence:
- Sloupce: hrany
- Řádky: vrcholy
(V každém sloupci jsou právě dvě jedničky)

Sled > Tah > Cesta

Dijkstraův algoritmus – nejkratší cesta
- Uzavřu ten vrchol, který je aktuálně nejblíž.
- Prohledám nově dostupné vrcholy a aktualizuji ceny.

Kruskalův algoritmus 
- Beru nejlevnější hrany, ale nikdy nesmím vytvořit cyklus.