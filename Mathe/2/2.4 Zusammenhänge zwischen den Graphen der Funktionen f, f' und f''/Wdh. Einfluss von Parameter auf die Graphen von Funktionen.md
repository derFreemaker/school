## $f(x) = a \cdot u(x)$
z.B.
- $f(x) = 3x^2$
- $f(x) = 4 \sin(x)$
- $f(x) = -\frac12 \cos(x)$

> [!note]
> $a$ bewirkt immer eine Streckung oder Stauchung in $y$-Richtung.
> 
> $a > 1 \implies$ Streckung
> $a < 1 \implies$ Stauchung
> 
> Für negative Werte von $a$ findet zusätzlich eine Spiegelung an der $x$-Achse statt.

## $f(x) = u(b \cdot x)$
z.B.
- $f(x) = \sqrt{5 \cdot x}$
- $f(x) = \sin(-2 \cdot x)$
- $f(x) = \cos(\frac{1}{3} \cdot x)$

> [!NOTE]
> $b$ bewirkt immer eine Streckung oder Stauchung in $x$-Richtung.
> 
> $b > 1 \implies$ Stauchung
> $b < 1 \implies$ Streckung
> 
> Für negative Werte von $b$ findet zusätzlich eine Spiegelung an der $y$-Achse statt.

> [!tip]
> Für $\sin$ und $\cos$ ist kleinste Periode $2\pi / b$.
## $f(x) = u(x +c)$
z.B.
- $f(x) = (x -4)^2$
- $f(x) = \sin(x + 2)$
- $f(x) = \sqrt{x -\frac12}$

> [!NOTE]
> $c$ bewirkt immer eine Verschiebung entlang der $x$-Achse.
> $c > 0 \implies$ nach links
> $c < 0 \implies$ nach rechts
## $f(x) = u(x) +d$
z.B.
- $f(x) = x^3 +4$
- $f(x) = \sin(x) - \frac32$
- $f(x) = \cos(x) +3$

> [!NOTE]
> $d$ bewirkt immer eine Verschiebung entlang der $y$-Achse.
> $d > 0 \implies$ nach oben
> $d < 0 \implies$ nach unten

## Beispiel 1
$fa(x) = \frac xa + \frac ax$ $a \neq 0$
#### Extrempunkte
$fa(x) = \frac 1ax + a \cdot x^{-1}$
$fa'(x) = \frac1a -a\cdot x^{-2}$

$0 = \frac1a -\frac{a}{x^2}$
$\frac{a}{x^2} = \frac1a$
$a^2 = x^2$
$x_1 = a$ $x_2 = -a$

$fa''(x) = 2a \cdot x^{-3} = \frac{2a}{x^3}$
$fa''(-a) = -\frac{2}{a^2} < 0 \implies Max(-a|-2)$
$fa''(a) = \frac{2a}{a^3} = \frac{2}{a^2} > 0 \implies Min(a|2)$

### Wendepunkte
$fa''(x) = \frac{2a}{x^3}$
$0 \neq \frac{2a}{x^3} \implies$ hat keine Wendepunkte

## Beispiel 2
$f_t(x) = \frac34x^3 -\frac32tx^2 +\frac34t^2x$ $t \neq 0$

### Achsenschnittpunkte
$0 = \frac34x^3 -\frac32tx^2 +\frac34t^2x$
$0 = \frac34x(x^2 -2tx +t^2)$
$x_1 = 0$
$x_{2;3} = t \pm \sqrt{t^2 - t^2}$
$x_2 = t$
$S_y = S_{x_1}(0|0)$ $S_{x_2}(t|0)$

#### Extrempunkte
$f_t'(x) = \frac94x^2 -3tx +\frac32t^2$

$0 = \frac94x^2 -3tx +\frac32t^2$
$0 = x^2 -\frac{4}3tx +\frac{2}{3}t^2$
$x_{1;2} = \frac23t \pm \sqrt{\frac49t^2 -\frac23t^2}$
$x_{1;2} = \frac23t \pm \sqrt{\frac19t^2}$
$x_{1;2} = \frac23t \pm \frac13t$
$x_1 = \frac13t$
$x_2 = t$

$f_t''(x) = \frac{9}{2}x -3t$

$f_t''(\frac13t) = \frac92 \cdot \frac13t -3t = -\frac32t \neq 0 \implies E_1(\frac13t|\frac19t^3)$
$f_t(\frac13t) = \frac34 \cdot \frac1{27}t^3 -\frac32 \cdot \frac19t^3 +\frac34 \cdot \frac13t^3 = \frac1{36}t^3 -\frac16t^3 +\frac14t^3 = \frac{1 -6 +9}{36}t^3 = \frac4{36}t^3 = \frac19t^3$
bei $t > 0$ ein Maximumpunkt
bei $t < 0$ ein Minimumpunkt

$f_t''(t) = \frac92t -3t = \frac32t \neq 0 \implies E_2(t|0)$  
$f_t(t) = \frac34t^3 -\frac32t^3 +\frac34t^3 = 0$
bei $t > 0$ ein Minimumpunkt
bei $t < 0$ ein Maximumpunkt

#### Wendepunkte und Wendetangente
$f_t''(x) = 0$
$0 = \frac92x -3t$
$\frac92x = 3t$ $| \cdot \frac29$
$x = \frac23t$

$f_t'''(x) = \frac92 \neq 0 \implies W_1(\frac23t|\frac1{18}t^3)$
$f_t(\frac23t) = \frac34 \cdot \frac8{27}t^3 -\frac32 \cdot \frac49t^3 +\frac34 \cdot \frac23t^3 = \frac29t^3 -\frac23t^3 +\frac12t^3 = \frac{4 -12 +9}{18}t^3 = \frac{1}{18}t^3$

$f_t'(\frac23t) = \frac94 \cdot \frac49t^2 -3 \cdot \frac23t^2 +\frac32t^2 = t^2 -2t^2 +\frac34t^2 = -\frac{1}{4}t^2$
$\frac1{18}t^3 = -\frac14t^2 \cdot \frac23t +n$
$n = \frac1{18}t^3 +\frac16t^3 = \frac4{18}t^3 = \frac29t^3$
$t: y = -\frac14t^2 \dot x +\frac29t^3$

#### Monotonie und Krümmungsverhalten
##### für $t > 0$:

| $x = \frac13t$ | $x = \frac23t$ | $x = t$ |
| -------------- | -------------- | ------- |
| Max            | W              | Min     |

für $x \leq \frac13t$ monoton steigend
für $\frac13 t \leq x \leq t$ monoton fallend
für $t \leq x$ monoton steigend

für $x < \frac23t$ rechtsgekrümmt
für $\frac23t < x$ linksgekrümmt

##### für $t < 0$:

| $x = t$ | $x = \frac23t$ | $x = \frac13t$ |
| ------- | -------------- | -------------- |
| Max     | W              | Min            |

für $x \leq t$ monoton steigend
für $t \leq x \leq \frac13t$ monoton fallend
für $\frac13t \leq x$ monoton steigend

für $x < \frac23t$ rechtsgekrümmt
für $\frac23t < x$ linksgekrümmt
