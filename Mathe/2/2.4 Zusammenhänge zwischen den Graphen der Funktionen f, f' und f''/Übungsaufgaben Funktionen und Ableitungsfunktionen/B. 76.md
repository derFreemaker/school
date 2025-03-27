# Nr. 5 - ohne CAS
## a)
$f_{z}(x) = x^3 -3zx^2 + (3z^2 -4)x -z^3 + 6z = x^3 -3zx^2 +3z^2x -4x -z^3 +6z$
$f_{z}'(x) = 3x^2 -6zx +3z^2 -4$
$f_{z}''(x) = 6x -6z$

$6x -6z = 0$
$x = z$

$f_{z}'''(x) = 6$
$f_{z}'''(z) = 6 \neq 0 \implies W(z|2z)$
$f_{z}(z) = z^3 -3z^3 +3z^3 -4z -z^3 +6z$
$f_{z}(z) = 2z$

$W(x) = 2x$

## b)
$f_{b}(x) = \frac{1}{b}x(x+b)^2$; $b \in \mathbb{R}_{-}$
$f_{b}(x) = (xb^{-1})x^2 + (xb^{-1})b^2$
$f_{b}(x) = x^3b^{-1} + xb$

$f_{b}'(x) = 3x^2b^{-1} +b$
$0 = 3x^2b^{-1} +b$ $|:3$
$0 = x^2b^{-1} +\frac{b}{3}$ $|\cdot b$
$0 = x^2 +\frac{b^2}{3}$
$x_{1;2} = -\frac{1}{2} \pm \sqrt{ \frac{1}{4} -\frac{b^2}{3} }$
$x_{1;2} = -\frac{1}{2} \pm \frac{1}{2} -\frac{b}{3}$
$x_{1} = -1 -\frac{b}{3}$
$x_{2} = -\frac{b}{3}$

$f_{b}''(x) = \frac{6x}{b}$
$f_{b}''\left( -1-\frac{b}{3} \right) = \frac{6\left( -1 -\frac{b}{3} \right)}{b} = \frac{-6 -\frac{6b}{3}}{b} = \frac{-\frac{6b}{3} +6}{b}$
???

keine Parameter

## c)
$f_{p}(x) = (x^2 -2x -p +2)e^x$

$f_{p}'(x) = (2x -2)e^x + (x^2 -2x -p +2)e^x$

???

// $0 = 2x -2$
// $x = 1$

// $f_{p}''(x) = 2e^x$
// $f_{p}''(1) = 2e \implies Min(1|e -ep)$
// $f_{p}(1) = e -ep$

// $T(x) = e-ex$

## d)
$f_{t}(x) = \sin(x) +\frac{x}{t}$; $x\in[0; 2\pi]$
$f_{t}(x) = \sin(x) +xt^{-1}$

$f_{t}'(x) = \cos(x) -t$
$f_{t}''(x) = -\sin(x)$
$0 = -\sin(x)$
$sin(x) = 0 \implies x_{1} = 0; x_{2} = \pi; x_{3} = 2\pi$

$f_{t}'''(x) = -\cos(x)$
$f_{t}'''(0) = -1 \neq 0 \implies W\left( 0| \frac{\pi}{t} \right)$
$f_{t}'''(\pi) = 1 \neq 0 \implies W\left( \pi|\frac{\pi}{t} \right)$
$f_{t}'''(2\pi) = -1 \neq 0 \implies W\left( 2\pi| \frac{\pi}{t} \right)$

$W(x) = \frac{\pi}{x}$

# Nr. 6a - mit CAS
- $S_{x}, S_{y}$
- $H, T$
- $W$
- Asymptoten
- Ortskurve der Extrempunkte

$f_{k}(x) = (k-x)e^x$; $k \in \mathbb{R}$

$0 = f_{k}(x)$
$S_{x}(k|0)$

$f_{k}(0) = k$
$S_{y}(0|k)$

$\underset{x\to-\infty}\lim{f_k(x)}=0 \implies$ waggerechte Asymptote $y=0$
keine senkrechte Asymptoten, da keine Definitionslücke(n)

$0 = f_{k}'(x)$
$x = k-1$
$f_{k}''(k-1) < 0 \implies H(k-1|-e^{k-1})$

$0 = f_{k}''(x)$
$x = k-2$
$W(k-2|-e^{k-2})$

$H(x) = -e^{x-2}$
