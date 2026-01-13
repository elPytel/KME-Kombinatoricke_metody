# Zápočtový test

Jaroslav Körner

Každý student má jednoznačně přiděleno číslo m, které je parametrem řešených úloh. Číslo m určí student ze vztahu m = 3 + (NNN mod 5), kde NNN je poslední trojčíslí osobního čísla studenta a (NNN mod 5) je nejmenší nezáporný zbytek čísla NNN modulo 5. 

1. Nalezněte řešení rekurentního vztahu $4𝑎_{𝑛+2} + 𝑎_𝑛 = 210$ vyhovující podmínkám:
   - $𝑎_0 = 2𝑚$,
   - $𝑎_1 = 3𝑚$. 
2. Uvažujte čtvercovou síť, ve které se lze pohybovat pouze pomocí kroků typu:
   - $A: [x,y]→[x+1,y]$, 
   - $B:[x,y]→[x,y+1]$. 
    Určete, kolika různými způsoby se lze dostat z bodu $[0,0]$ do $[11,11]$ tak, že nepřekročíte diagonálu a neprojdete žádným z bodů $[m,m]$ nebo $[11-m,11-m]$. 

3. Nalezněte uzavřený tvar obyčejné vytvořující funkce posloupnosti
$$
𝑎_𝑛 = (𝑚 + 1) * 𝑛 * (\frac{2}{3})^𝑛
$$
4. Určete počet celočíselných řešení rovnice:
$$
𝑥_1 + 𝑥_2 + 𝑥_3 + 𝑥_4 + 𝑥_5 = 28
	$$které vyhovují podmínkám:
- $𝑚 ≤ 𝑥1 ≤ 𝑚 + 6$;
- $−3 ≤ 𝑥2$; 
- $−2 ≤ 𝑥3$; 
- $4 ≤ 𝑥4 ≤ 10$; 
- $2 ≤ 𝑥5 ≤ 9$ 
---
## Číslo studenta
M23000127

$m = 3 + (127 mod 5)$
$m = 3 + 2$
$m = 5$

---
## Rekurentní vztah
$$
4𝑎_{𝑛+2} + 𝑎_𝑛 = 210
$$ vyhovující podmínkám:
   - $𝑎_0 = 2*5 = 10$,
   - $𝑎_1 = 3*5=15$. 

char. polynom:
$4x^{n+2}+x^{n} = 0$
$x^{n}*(4x^2+1) = 0$

$D = \sqrt{0^2-4*4*1} = \sqrt{-16} = \sqrt{j^2*4^2} = 4j$
$x_{1,2} = \frac{-0 \pm \sqrt{0^2-4*4*1} }{2*4} = \pm 4j/8$
$x_{1,2} = \pm 1/2j$

Homogenní řešení:
$x_{1,2} = re^{\pm j\theta}$
kde:
- $r=1$
- $\theta = \frac{\pi}{2}$ (protože $\frac{1}{2} j = e^{i \frac{\pi}{2}}$​)
$$
a_n^h​=K_1(​r)^ncos(n\theta)+K_2(​r)^nsin(n\theta)
$$
$$
a_n^h = K_1(1)^n*cos(n\pi/2) + K_2(1)^n​sin(n\pi/2​)
$$

Partikulární řešení:
Pravá strana není závislá na n, jde o konstantu. Hledáme řešení ve tvaru konstanty:
$a_n^p = C$

$4C+C=210$
$5C=210$
$a_n^p=42$

$$
a_n = K_1*cos(n\pi/2) + K_2sin(n\pi/2​) + 42
$$
Použijeme počáteční podmínky:
- $a_0 = 10 = K_1 + 42$
	- $K_1 = -32$
- $a_1=15 = K_2 +42$
	- $K_2 = -27$

Výsledné řešení:
$$
a_n = -32*cos(n\pi/2) - 27sin(n\pi/2​) + 42
$$
---

## Kroky v čtvercové síti
Uvažujte čtvercovou síť, ve které se lze pohybovat pouze pomocí kroků typu:
   - $A: [x,y]→[x+1,y]$, 
   - $B:[x,y]→[x,y+1]$. 
Určete, kolika různými způsoby se lze dostat z bodu $[0,0]$ do $[11,11]$ tak, že nepřekročíte diagonálu a neprojdete žádným z bodů $[5,5]$ nebo $[6,6]$. 

Princip inkluze a exkluze:



---
## Volitelné úlohy 
### Rozhodněte, zda zobrazený graf je rovinný. 

![[Graf.png|300]]

Pokud graf obsahuje jako svůj podgraf graf $K_5$ (úplný graf o 5 vrcholech), pak není rovinný.
![[Complete_graph_K5.svg.png|300]]
Když sloučíme vrcholy z vrcholu hvězdice a s příslušné vrcholy pěti-úhelníku. Tak transformujeme graf ze zadání na graf $K_5$, ten rovinný není, ani původní graf tedy není rovinný. 

### Určete, kolik existuje 𝑘-prvkových podmnožin množiny $𝑆 = \{1, … , 𝑛\}$, které neobsahují žádná dvě po sobě jdoucí přirozená čísla. 

### Na kružnici rozmístíte $2𝑛$ různých bodů. Určete, kolika různými způsoby lze pomocí neprotínajících se tětiv spojit dvojice bodů.

Rozdělíme úlohu na pod části:
1) Spojování bodů postupně kolem dokola.
2) Propojování bodů jeden se všemi ostatními.
3) Nakonec odstraníme překrývající se tětivy.

1) Pro 2n bodů vznikne 2n různých tětiv.
2) 1 bod s každým: 2n-1 tětiv
3) Dvě tětivy se překrývají (dva nejbližší body po stranách téhož ze kterého propojujeme ostatní): -2

 $a_n = 2n + 2n-1 -2 = 4n -3$

| n   | počet bodů | počet tětiv |
| --- | ---------- | ----------- |
| 1   | 2          | 1           |
| 2   | 4          | 4+(4-1)-2=5 |
| 3   | 6          | 6+(6-1)-2=9 |

