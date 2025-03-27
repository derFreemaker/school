
$f(x)=\frac{a_nx^n+a_{n-1}x^{n-1}+...+a_1x+a_0}{b_mx^m+b_{m-1}x^{m-1}+...+b_1x+b_0}$ $a_n\neq0, b_m\neq0, m>0$

- Für $n<m$ gilt $\underset{x\rightarrow\pm\infty}\lim{f(x)}=0$
- Für $n=m$ gilt $\underset{x\rightarrow\pm\infty}\lim{f(x)}=\frac{a_n}{b_m}$
- Für $n>m$ gilt es gelten keine Grenzwerte nur uneigentliche Grenzwerte $+\infty$ oder $-\infty$.


| $\underset{x\rightarrow-\infty} \lim f(x)$ | $n-m$ gerade | $n-m$ ungerade |
| ------------------------------------------ | ------------ | -------------- |
| $\frac{a_n}{b_n}>0$                        | $+\infty$    | $-\infty$      |
| $\frac{a_n}{b_n}<0$                        | $-\infty$    | $+\infty$      |

| $\lim f(x)$<br>$x\rightarrow+\infty$ | $n-m$ gerade | $n-m$ ungerade |
| ------------------------------------ | ------------ | -------------- |
| $\frac{a_n}{b_n}>0$                  | $+\infty$    | $+\infty$      |
| $\frac{a_n}{b_n}<0$                  | $-\infty$    | $-\infty$      |

## Asymptote

### a)
Aus dem Verhalten im Unendlichen lassen sich Aussagen zu waagerechten Asymptoten ableiten.

#MatheDefinition 4:
Eine waagerechte Asymptote ist der Graph einer Funktion ($f(x)=g$) die sich immer weiter annähert ohne sich im Unendlichen zu erreichen.
```
a-syn-piptein
```

### Beispiel 1
$f(x)=\frac{2x-3}{x^2+4}$
- $\underset{x\to\pm\infty}\lim{f(x)}=0$

### Beispiel 2
$f(x)=\frac{4x^2-3}{x^2+5}$
- $\underset{x\to\pm\infty}\lim{f(x)}=4$ => waagerechter Asymptote y=4

### Beispiel 3
$f(x)=\frac{2x-3}{\mid x-1 \mid}$
- $\underset{x\to+\infty}\lim{f(x)}=2$ => waagerechter Asymptote y=2
- $\underset{x\to-\infty}\lim{f(x)}=-2$ => waagerechter Asymptote y=-2


> [!IMPORTANT] #MatheMerke
> Eine gebrochene rationale Funktionen haben maximal zwei verschiedene Asymptote haben.

### b)
Verhalten an einer Stelle $x_0$


> [!NOTE] #MatheDefinition 5
> Eine Zahl $g$ heißt Grenzwert einer Funktion $f$ an einer Stelle $x_0$, wenn für jede Zahlenfolge ($x_n$) mit $x_n\epsilon D_f$ und $x_n\neq x_0$, die gegen $x_0$ konvergiert, die zugehörige Bildfolge ($f(x_n)$) gegen $g$ konvergiert.

$\underset{x\to x_0}\lim{f(x)}=g$
### Beispiel
$f(x)=7-5x$, Stelle $x_0=2$

| Zahlenfolge<br>($x_n$)      | $x_1$<br>$1,9$     | $x_2$<br>$1,99$     | $x_3$<br>$1,999$     | $x_4$<br>$1,9999$     | $x_5$ -> $x_0$<br>$1,99999$ -> 2      |
| --------------------------- | ------------------ | ------------------- | -------------------- | --------------------- | ------------------------------------- |
| **Bildfolge**<br>($f(x_n)$) | $f(x_1)$<br>$-2,5$ | $f(x_2)$<br>$-2,95$ | $f(x_3)$<br>$-2,995$ | $f(x_4)$<br>$-2,9995$ | $f(x_5)$ -> $g$<br>$-2,99995$ -> $-3$ |
#### Einsatz im CAS
$\lim(f(x), x, x_0)$
oder
$\underset{x\to x_0}\lim{f(x)}$

### Beispiel
$f(x)=\frac{4x+4}{\mid x+1 \mid}$
$y=/$

#MatheDefinition 6:
- $\underset{x\to x_0, x<x_0}\lim{f(x)}=\underset{x\to x_0-0}\lim{f(x)}$ wird als linksseitiger Grenzwert von $f$ an der Stelle $x_0$ bezeichnet. ($x_n < x_0$)

- $\underset{x\to x_0, x>x_0}\lim{f(x)}=\underset{x\to x_0+0}\lim{f(x)}$ wird als rechtsseitiger Grenzwert von $f$ an der Stelle $x_0$ bezeichnet. ($x_n > x_0$)

#### Einsatz im CAS 
- rechtsseitiger
	$lim(f(x),x,x_0,\text{neg.Wert})$
	$\underset{x\to x_0-}\lim{f(x)}$
- linksseitiger
	$lim(f(x),x,x_0,\text{pos.Wert})$
	$\underset{x\to x_0+}\lim{f(x)}$

### Beispiel

$f(x)=\frac{4x+4}{\mid x+1 \mid}$
- $\underset{x\to-1}\lim{f(x)}$ existiert nicht
- $\underset{x\to-1-0}\lim{f(x)}=-4$
- $\underset{x\to-1+0}\lim{f(x)}=+4$


> [!IMPORTANT] #MatheMerke
> Wenn der linksseitige Grenzwert an einer Stelle ungleich dem rechtsseitigen Grenzwert an dieser Stelle ist, dann existiert der Grenzwert an dieser Stelle nicht.
> $\underset{x\to x_0-0}\lim{f(x)}\neq\underset{x\to x_0+0}\lim{f(x)}$

Wenn der linksseitige Grenzwert an einer Stelle gleich dem rechtsseitigen Grenzwert an dieser Stelle ist, dann existiert der gemeinsame Grenzwert an dieser Stelle.
$\underset{x\to x_0-0}\lim{f(x)}=\underset{x\to x_0+0}\lim{f(x)}\implies\underset{x\to x_0}\lim{f(x)}$

Grenzwerte einer Funktion an einer Stelle ist $0$. Liefern Aussagen über den Verlauf des Graphen an dieser Stelle.

#MatheDefinition 7:
Die Funktion $f$ heißt **stetig** an der Stelle $x_0$, wenn:
1. $f$ an der Stelle $x_0$ einen Funktionswert besitzt.
2. $f$ an der Stelle $x_0$ einen Grenzwert besitzt.
3. $f(x_0)=\underset{x\to x_0}\lim{f(x)}$ gilt.

### Unstetigkeitsstellen
#### a) Hebbare Lücken
1. Hebbare Lücke heißt die Funktion $f$ kann an der betroffenen Stelle einen Funktionswert besitzen muss es aber nicht.
2. Es existiert mindestes einer der beiden einseitigen Grenzwerte.

#### b) Polstellen
1. Die Funktion besitzt an dieser Stelle keinen Funktionswert.
2. Es existiert auch keiner der beiden einseitigen Grenzwerte, sondern nur uneigentliche Grenzwerte $+\infty$ und $-\infty$.

#MatheDefinition 8:
Ist $x_{p}$ einer Polstelle der Funktion $f$, dann bezeichnet man die Gerade mit der Gleichung $x=x_{p}$ als **senkrechte Asymptote** (Polasymptote, Polgerade) von $f$.

#### Beispiel

$f(x)=\frac{x^4-7x^3+17x^2-17x+6}{x^4-5x^3+x^2+21x-18}$
alle waagerachten und senkrechten Asymptote

$\underset{x\to+\infty}\lim{f(x)}=1$ -> waagerechte Asymptote $y=1$

$x^4-5x^3+x^2+21x-18=0$
$x_1=-2$
$x_2=1$
$x_3=3$

$\underset{x\to-2-0}\lim{f(x)}=+\infty$
$\underset{x\to-2+0}\lim{f(x)}=-\infty$ -> senkrechte Asymptote $x=-2$

$\underset{x\to1-0}\lim{f(x)}=0$ -> hebbare Lücke

$\underset{x\to3-0}\lim{f(x)}=-\infty$
$\underset{x\to3+0}\lim{f(x)}=+\infty$ -> senkrechte Asymptote $x=3$

