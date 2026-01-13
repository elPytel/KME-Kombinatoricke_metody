# Příklady ze cvičení

- [[KME_příklady_gen_fnc_web.pdf]]
- [[KME_příklady_rekurent_web.pdf]]
- [[KME_příklady_elem_komb_web.pdf]]

## Zápis v Latechu
$$
\binom{5}{6} \binom{5}{2}
$$


$$
\begin{array}{c} 12 \\ 34 \end{array}
$$

# K Zamyšlení:
## 1.

$$
S_n = min \{
k \in N^+\ | 
A_1, ..., A_n \subset \{1,2,...,k \}
\}
$$
$$
\cup A_i = \{1,2,3,...,k\} \land \forall i,j \; A_i \land A_j \neq \emptyset
$$

Existuje $A_i$ takové, že rovnice:

$$
x+y=z
$$
Má řešení v $A_i$.

## 2.
Posloupnosti: $a_1,...,a_k$
- $a_1 = 1$
- $a_k = N$
- $a_i \in N$
- $\forall a_i \le a_{a+i}$ - rostoucí posloupnost

Kolik existuje posloupností s výše uvedenou vlastností?

## 3.
Určete počet bitových řetězců délky n, které obsahují sekvenci "01".

Určete počet slov délky n nad abecedou (0,1,2), které neobsahují 2 po sobě jdoucí nuly, nebo dvě po sobe jdoucí jedničky.
# Rekurentní vztahy
## Příklad
Rekurentní vztah:
$$
a_n = 8a_{n-1} - 16 a_{n-2}
$$
Je posloupnost řešením rekurentního vztahu?

| Posloupnost           | Je řešením? |
| --------------------- | ----------- |
| $a_n = 0$             |             |
| $a_n = 1$             |             |
| $a_n = 2^n$           |             |
| $a_n = 4^n$           |             |
| $a_n = n4^n$          |             |
| $a_n = 2*4^n + 3n4^n$ |             |
| $a_n = -4^n$          |             |
| $a_n = n^2*4^n$       |             |
### Postup

$(x^2-8x+16) = 0$
$(x-4)^2$
$x =4$

#TODO
### Řešení
| Posloupnost           | Je řešením? |
| --------------------- | ----------- |
| $a_n = 0$             | ano         |
| $a_n = 1$             | ne          |
| $a_n = 2^n$           | ne          |
| $a_n = 4^n$           | ano         |
| $a_n = n4^n$          | ano         |
| $a_n = 2*4^n + 3n4^n$ | ano         |
| $a_n = -4^n$          | ne          |
| $a_n = n^2*4^n$       | ne          |

## Zásobník

push ->
pop <-

$C_n$ - kolik různých n-tic realizovatelných pomocí zásobníku

- $c_1 = 1$
- $c_2 = 2$
- $c_3 = 6$

Sestavte si rekurentní vztah:

# Další
## Příklad

### Postup

### Řešení
# Další

## Cvičení 1.3.3. 
V jedné řadě je 9 volných míst. Kolika způsoby na ně můžeme rozesadit 6 studentů a 3 profesory tak, aby každý profesor seděl mezi dvěma studenty? (Studenti musejí sedět hned vedle profesora.)
### Postup

### Řešení

## Cvičení 1.3.4. 
Přirozené číslo d nazveme vzestupné, pokud jeho ciferný zápis má tvar:
$$d_md_{m-1}...d_2d_1$$
kde: 
$$
d_m \leq d_1 \leq ... \leq d_2 \leq d_1
$$
(Např. číslo 11334 je vzestupné.) Kolik existuje vzestupných přirozených
čísel menších než 10100?
### Postup

### Řešení

## Cvičení 1.3.5 Narozeninový paradox
Jaká je pravděpodobnost, že mezi n náhodně vybranými osobami budou alespoň dva lidé, kteří mají narozeniny ve stejný den? 
Jak velké musí být n, aby tato pravděpodobnost přesáhla 1/2? 
Předpokládejte, že všechna data narození jsou stejně pravděpodobná. K zodpovězení druhé otázky použijte počítač.
### Postup

Dní v roce: 366


Počet všech možností:
$366^n$

Pravděpodobnost:
$P =$
### Řešení
$$P = 1 − 366 · 365 · · ·(367 − n)/366^n$$

## Příklady
A: Permutace
1) Určete, kolik 5ti ciferných čísel lze zapsat pomocí číslic 0, 1, 2, 3, 4?
2) Kolikerým způsobem lze rozsadit 12 žáků ve třídě?
3) Kolik různých 4ciferných čísel lze utvořit z čísel 1,4,7,9?
4) Kolik různých 6ticiferných čísel se dá napsat dvěma pětkami a čtyřmi šestkami? Napište je.
5) V lavici sedí pět žáků, A,B,C,D, E. Kolikrát je lze přesadit tak a) aby, žák A byl krajní, b) aby žáci A a B seděli vedle sebe?
6) Kolik různých melodií je možno utvořit ze 6ti různých tónů?
7) Kolik různých signálů lze dát čtyřmi různými vlaječkami?
8) Kolik různých 5ticiferných čísel se dá napsat užitím dvou nul, dvou trojek a jedné šestky?
9) Kolik sedmimístných čísel lze zapsat číslicemi 7, 8, 9, 9, 0, 0, 0.
10) Zvětšíme-li počet prvků o dva, zvětší se počet permutací dvanáctkrát. Kolik prvků bylo dáno?
11) Zmenšíme-li počet prvků o dva, zmenší se počet permutací dvacetkrát. Určete, původní počet prvků.

B: Variace
1) Kolik variací druhé, třetí, čtvrté třídy a) bez opakování, b) s opakováním bude ze 7mi a kolik ze 12ti prvků?
2) Kolik trojciferných čísel se dá napsat číslicemi 2, 5, 6, 8, 9?
3) Kolik trikolor lze sestavit ze 7mi různých barev?
4) Kolik tříčlenných skupin lze sestavit ze sedmi žadatelů?
5) Osm spolužáků se dohodlo při odchodu na prázdniny, že si pošlou navzájem pohlednice z cest. Kolik pohlednic bylo celkem rozesláno?
6) Ve škole se učí 12ti různých předmětům a každému se učí nejvýš 1 vyučování hodinu denně. Kolikerým způsobem je možno sestavit rozvrh hodin na jeden den, je-li toho dne 6 různých předmětů?
7) Kolik 4ciferných čísel lze sestavit z devíti arabských číslic bez nuly a) aby čísla obsahovala různé číslice, b) číslice se mohou opakovat.
8) Kolik různých (jedno až pěticiferných) přirozených čísel lze napsat číslicemi 0, 1, 2, 3, 4, nemá-li  se v žádném čísle žádná číslice opakovat?
9) Z kolika prvků lze utvořit 420 variací druhé třídy bez opakování?
10) Kolik telefonických hovorů lze uskutečnit mezi 20ti účastníky?
11) Kolik různých vrhů je možno učinit a) dvěma, b) třemi hracími kostkami?
12) Vypočtěte x, je-li .

C: Variace a permutace
1) V lavici mohou sedět 4 žáci, Kolikerým způsobem lze lavici obsadit pěti žáky, jestliže záleží na pořadí míst?
2) Kolik a) dvojciferných, b) trojciferných, c) čtyřciferných čísel je možno napsat číslicemi 1, 3, 5, 7, 9 tak, aby se ani jedna číslice neopakovala?
3) Kolik různých čísel můžeme napsat z číslic 1, 2, 3, 4, 5, 6 má-li se každá číslice vyskytnout v čísle pouze jednou?
4) Kolik trojciferných čísel je možno naspat číslicemi 2, 4 ,6, 8, mohou-li se číslice opakovat?
5) Z kolika prvků možno utvořit a) 42, b) 56 variací druhé třídy bez opakování?
6) Kolik je třeba prvků, aby počet variací druhé třídy byl dvacetkrát menší než počet variací čtvrté třídy.
7) Z kolika prvků vznikne a) 729 variací třetí třídy s opakováním, b) 1024 variací páté třídy s opakováním.
8) Kolik permutací bez opakování je možno utvořit z prvků a, b, c, d, e, f, g tak, aby
	a) všechny začínaly prvkem a,
	b) všechny začínaly skupinou abc,
	c) všechny začínaly prvkem a a končily prvkem g,
	d) prvky b, d, f neměnily své místo,
	e) prvky a, b, c byly stále spolu, ale v libovolném pořadí.
9) Aranžér má ve výkladě umístit vedle sebe 4 stejné svetry, z nichž jsou dva bílé, jeden červený a jeden zelený. Kolik způsoby to může učinit?
10) Kolik čísel je možno napsat číslicemi 0, 3, 4, 5, 7 (číslice se neopakují) a) různých, b) dělitelných 2, 
c) dělitelných 10, d) dělitelných 5?
11) Kolik pěticiferných čísel je možno sestavit z 0, 1, 3, 4, 7? Kolik z nich je lichých? Číslice se neopakují.

Výsledky:
A: 1) 96, 2) 12!, 3) 24, 4) 15, 5) a) i b) 48, 6) 720, 7) 24, 8) 18, 9) 240, 10) 2, 11) 5
B: 1) a) 42, 210, 840; 132, 1320, 11880, b) 49, 343, 2401; 144, 1728, 20736, 2) 60, 3) 210, 4) 210, 5) 56, 
6) 665280, 7) a) 3024, b) 6561, 8) 260, 9) 21, 10) 380, 11) a) 36, b) 216, 12) 8
C: 1) 120, 2) a) 20, b) 60, c) 120, 3) 1956, 4) 64, 5) a) 7, b) 8, 6) 7, 7) a) 9, b) 4, 8) a) 720, b) 24, c) 120, 
d) 24, e) 720, 9) 12, 10) a) 96, b) 42, c) 24, d) 42, 11) 96, 54
