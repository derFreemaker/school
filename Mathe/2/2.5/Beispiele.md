# Beispiel 1
#### Form
$ax^3 +bx^2 +cx +d$
#### $H(3|2)$
$f(3) = 2$
$f'(3) = 0$

#### $W(2|f(2))$
$f''(2) = 0$

#### $m_{W} = 1.5$
$f'(2) = 1.5$

$f(x) = -\frac{1}{2}x^3 + 3x^2 -\frac{9}{2}x +2$

- Probe Text
- Probe Bedingungen mit Grafik vergleichen

# Beispiel 2
#### Form
$ax^4 +bx^3 +cx^2 +dx +e$

#### $S(0|0)$
$f(0)=0$
$f'(0)=0$
$f''(0)=0$

#### $W(1|1)$
$f(1)=1$
$f''(1)=0$

$-x^4 +2x^3$

# Beispiel 3

#### Form:
$ax^4 +bx^2 +c$

#### Bedingungen:
  I. $f(2) = -\frac{20}{3}$
 II. $f''(2) = 0$
III. $f'(2) = -\frac{16}{3}$

#### Lösung:
$f'(x) = 4ax^3 +2bx$
$f''(x) = 12ax^2 +2b$

  I. $f(2) = 16a +4b +c = -\frac{20}{3}$
 II. $f''(2) = 48a +2b = 0 \implies b = -24a$
III. $f'(2) = 32a +4b = -\frac{16}{3}$
#### 1. Einsetzen
$32a -96a = -\frac{16}{3}$
$64a = -\frac{16}{3}$
$a = -\frac{16}{3}\cdot\left( -\frac{1}{64} \right)$
$a = \frac{1}{12}$
$b = -24\cdot \frac{1}{12} = -2$
$16\cdot \frac{1}{12} -8 +c = -\frac{20}{3}$
$c = -\frac{20}{3} -\frac{4}{3} +8 = 0$

$f(x) = \frac{1}{12}x^4 -2x^2$

#### 2. Gaußsches verfahren
$a$  $b$ $c$
$16$ $4$ $1$ | $-\frac{20}{3}$
$42$ $2$ $0$ | $0$
$32$ $4$ $0$ | $-\frac{16}{3}$

$\left|\begin{matrix} 16 & 4 & 1 \\ 48 & 2 & 0 \\ 32 & 4 & 0 \end{matrix}\right|\begin{matrix} -\frac{20}{3} & \frac{43}{3} \\ 0 & 50 & III' = 2\cdot II - III \\ -\frac{16}{3} & \frac{92}{3} \end{matrix}$

$\left|\begin{matrix} 16 & 4 & 1 \\ 48 & 2 & 0 \\ 64 & 0 & 0 \end{matrix}\right|\begin{matrix} -\frac{20}{3} & \frac{43}{3} \\ 0 & 50 \\ \frac{16}{3} & \frac{208}{3} \end{matrix}$

$64a = \frac{16}{3}$
$a = \frac{1}{12}$

$48a + 2b = 0$
$48\cdot \frac{1}{12} +2b = 0$
$4 + 2b = 0$
$b = -2$

$16a +4b +c = -\frac{20}{3}$
$16\cdot \frac{1}{12} -8 +c = -\frac{20}{3}$
$c = -\frac{20}{3} -\frac{4}{3} +8 = 0$
