
1. Menü Grafik & Tabelle
	- Analyse -> graf. Lösung -> Minimum | Maximum
#### Beispiel
$f(x) = \frac{1}{6258} \cdot (x -\frac{854}{13})^2$

> [!NOTE] Mögliche Probleme
> 1. Wenn Fenster Einstellungen ungünstig sind werden vorhandene Lösungen nicht gefunden.
> 2. Selbst wenn ich das richtige Fenster finde, bekomme ich nur ein Näherungswert.

2. Menü Main
	- $0 = \text{diff}(f(x), x)$
#### Beispiel
$f(x) = \frac{3x^2 -8x}{(x-2)^2}$

> [!tip] CAS
> 
> [Define](Befehle#Define) $f(x) = \frac{3x^2 -8x}{(x-2)^2}$

$f'(x) = 0$

> [!tip] CAS
> [diff](Befehle#diff)$(f(x), x)$

$x = 4$

> [!tip] CAS
> [solve](Befehle#solve)$(ans=0[,x])$

$f''(4) = -\frac12$

> [!tip] CAS
> [diff](Befehle#diff)$(f(x),x,2,4)$

$\implies Max(4|4)$


> [!tip] CAS
> $f(4)$

#### 1. Beispiel
$f(x) = \frac{1}{6258} \cdot (x -\frac{854}{13})^2$
$f'(x) = 0$
$x = \frac{854}{13}$
$f''(\frac{854}{13}) = \frac{122}{5811} \implies Min(\frac{854}{13}|0)$

#### 2. Beispiel
$f(x) = \frac{49}{15}x^3 +\frac{7}{3}x^2 -3x +1$
$f'(x) = 0$
$x_1 = -\frac57$
$x_2 = \frac37$

$f''(-\frac57) = -\frac{(98 \cdot x+14)}{7} \implies Max(-\frac57|\frac83)$
$f''(\frac37) = \frac{3 \cdot (98 \cdot x +14)}{35} \implies Min(\frac37|\frac{8}{35})$

#### 3. Beispiel
$f(x) = \frac{x}{a} + \frac{a}{x}$
$f'(x) = 0$
$x_1 = -a$
$x_2 = a$

$f''(-a) = -\frac{2 \cdot a^2}{x^3} \implies Max(-a|-2)$
$f''(a) = \frac{2 \cdot a^2}{x^3} \implies Min(a|2)$

## Übung
#### 1. $f(x) = \frac{9-x^2}{x^2+3}$
$f'(x) = 0$
$x = 0$

$f''(0) = -\frac83 < 0 \implies Max(0|3)$
#### 2. $f(x) = \frac{1}{4}x\cdot\sqrt{16 -x}$
$f'(x) = 0$
$x = \frac{32}{3}$

$f''(\frac{32}{3}) = -\frac{3\cdot\sqrt{3}}{32} < 0 \implies Max(\frac{32}{3}|\frac{32\cdot\sqrt{3}}{9})$
#### 3. $f(x) = (x^2+4x+4)\cdot e^{-x}$
$f'(x) = 0$
$x_1 = -2$
$x_2 = 0$

$f''(-2) = 2\cdot e^2 > 0 \implies Min(-2|0)$
$f''(0) = -2 < 0 \implies Max(0|4)$
#### 4. $f(x) = \frac{(x^2 -2) \cdot e^x}{1+e^x}$
$f'(x) = 0$
$x = \ln(\sqrt3-1)$

$f''(\ln(\sqrt3-1)) \approx 0.619 > 0 \implies Min(\ln(\sqrt3-1)|\frac{-\sqrt3\cdot(\sqrt3-1)\cdot(-\sqrt3+3))}{3})$
#### 5. $f(x) = 2\sin x -\cos(2x)$ im Intervall $-\frac{\pi}{3} \leq x \leq 3\pi$
   ([solve](Befehle#solve)$(f(x),x) | -\frac{\pi}{3} \leq x \leq 3\pi$)
$f'(x) = 0$
$x_1 = -\frac{\pi}{6}$
$x_2 = \frac{\pi}{2}$
$x_3 = \frac{3\cdot\pi}{2}$
$x_4 = \frac{5\cdot\pi}{2}$
$x_5 = \frac{7\cdot\pi}{6}$
$x_6 = \frac{11\cdot\pi}{6}$

$f''(-\frac{\pi}{6}) = 3 > 0 \implies Min(-\frac{\pi}{6}|-\frac{3}{2})$
$f''(\frac{\pi}{2}) = -6 < 0 \implies Max(\frac{\pi}{2}|3)$
$f''(\frac{3\cdot\pi}{2}) = -2 > 0 \implies Max(\frac{3\cdot\pi}{2}|-1)$
$f''(\frac{5\cdot\pi}{2}) = -6 < 0 \implies Max(\frac{5\cdot\pi}{2}|3)$
$f''(\frac{7\cdot\pi}{6}) = 3 > 0 \implies Min(\frac{7\cdot\pi}{6}|-\frac{3}{2})$
$f''(\frac{11\cdot\pi}{6}) = 3 > 0 \implies Min(\frac{11\cdot\pi}{6}|-\frac{3}{2})$

Zusatz: Welcher dieser Funktion können im A-Teil dran kommen?
1 und 2
