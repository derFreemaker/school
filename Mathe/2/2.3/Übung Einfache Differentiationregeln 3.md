## Aufgabe 1
$f(x) = x^3-\frac32x^2-5x+12$

$f'(x) = 3x^2-3x-5$
### a)
#### schriftliche Lösung
$-5 = 3x^2-3x-5$ $|+5$
$0 = 3x^2 - 3x$ $|$
$0 = 3x(x - 1)$
$x_1 = 0$ $x_2 = 1$

$f(0) = 12$
$12 = -5 * 0 + 4$
$n = 12$
$t_1 = -5x + 12$

$f(1) = 6.5$
$6.5 = -5x + 11.5$
$n = 11.5$
$t_2 = -5x + 11.5$

#### Lösung mit CAS
$-5 = f'(x)$
$x_1 = 0$ $x_2 = 1$

[tanline](Mathe/Befehle#tanline): $t_1 = -5x + 12$
[tanline](Mathe/Befehle#tanline): $t_2 = -5x + 11.5$

### b)
#### schriftliche Lösung
$-\frac{11}4 = 3x^2 - 3x - 5$ $|+\frac{11}4$
$0 = 3x^2 - 3x - \frac9{4}$ $|:3$
$0 = x^2 - x - \frac3{4}$
$x_{1,2} = \frac12 \pm \sqrt{\frac14 + \frac3{4}} = \frac12 \pm 1$
$x_1 = -\frac12$ $x_2 = \frac32$

$f(-\frac12) = 14$
$14 = \frac{11}{8} +n | -\frac{11}8$
$n = 14 -\frac{11}8$
$n = \frac{101}{8}$
$t_1 = -\frac{11}4x + \frac{101}{8}$

$f(\frac32) = 4.5$
$4.5 = \frac{55}8$

#### Lösung im CAS
$-\frac{11}4 = f'(x)$
$x_1 = -\frac12$ $x_2 = \frac32$

[tanline](Mathe/Befehle#tanline): $t_1 = $
[tanline](Mathe/Befehle#tanline): $t_1 = $

### c)
#### schriftliche Lösung
$+1 = 3x^2 - 3x - 5$ $|-1$
$0 = 3x^2 - 3x - 6$ $|:3$
$0 = x^2 - x - 2$ 
$x_{1,2} = \frac12 \pm \sqrt{\frac14 + 2} = \frac12 \pm 1.5$
$x_1 = -1$ $x_2 = 2$

$f(-1) = 14.5$
$14.5 = -1 + n \implies n = 15.5$
$t_1 = x + 15.5$

$f(2) = 4$
$4 = 2 + n \implies n = 2$
$t_2 = x + 2$

#### Lösung mit CAS
$+1 = f'(x)$
...

## Aufgabe 2
$f(x) = -\frac23x^2 -\frac83x +\frac{10}3$

$f'(x) = -\frac43x -\frac83$
### a)
$0 = -\frac23x^2 -\frac83x +\frac{10}3$ $|*3$
$0 = -2x^2 -8x + 10$ $|:2$
$0 = -x^2 -4x +5$ $|*-1$
$0 = x^2 + 4x - 5$
$x_{1,2} = -2 \pm 3$
$\underline{\underline{S_{x1} = 1}}$ $\underline{\underline{S_{x2} = -5}}$

$m_1 = f'(1)=−\frac{4}{3}(1) −\frac{8}{3}​= −\frac{4}{3}​ −\frac{8}{3}​= −\frac{12}{3}​=−4$
$m_2 = f(-5) = -\frac{4}{3}(-5) -\frac{8}{3} = \frac{20}{3} -\frac{8}{3} = \frac{12}{3} = 4$

$\arctan{\varphi} = |\frac{m2 - m1}{1 +m1*m2}| = \frac{8}{15}$
$\underline{\underline{\varphi \approx 28.072^\circ}}$

### b)
$y_1 = -4(x -1) = -4x +4$
$y_2 = 4(x + 5) = 4x +20$

$-4x + 4 = 4x + 20$ $|-4x;$ $-4$
$-8x = 16$ $|:-2$
$x = -2$

$y = -4(-2) + 4 = 12$
Schnittpunkt Tangenten: $P(-2; 12)$

$a = 1 - (-5) = 6$
$b = 12$
$A = \frac12*a*b = \underline{\underline{36FE}}$

## Aufgabe 3
$f(x) = \frac23x^2 -\frac53x +1$

$f'(x) = \frac43x -\frac53$

$y = f(\frac32) = 0$
$m_t = f'(\frac32) = \frac13$
$m_n = -\frac{1}{m_t} = -3$

$0 = -3*\frac32 +n$
$0 = -\frac92 +n$ $|+\frac92$
$\frac92 = n$
$y = -3x +\frac92$

$\underline{\underline{P(0, \frac92)}}$

$\arctan{3} \approx 71.57^\circ$
$90^\circ - 71.57^\circ = \underline{\underline{18.43^\circ}}$
## Aufgabe 4
$f(x) = \frac32\sin{x} +1$

$f'(x) = \frac32\cos{x}$

$y = f(2\pi) = 1$
$m_t = f'(2\pi) = \frac32$

$1 = \frac32(2\pi) +n$
$y = \frac32x -3\pi +1$
$0 = \frac32x -3\pi+1$ $|+3\pi-1$
$3\pi-1 = \frac32x$ $|*2;$ $:3$
$2\pi -\frac23 = x$

$\underline{\underline{S(2\pi -\frac23|0)}}$

$\underline{\underline{\arctan{m_t} = \arctan{\frac32} \approx 56.31^\circ}}$
