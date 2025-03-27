> [!tip] Notwendige Bedingung für Wendepunkte 
> $f''(x_W) = 0$

> [!tip] Hinreichende Bedingung für Wendepunkte
> $f'''(x_W) \neq 0$

#### Beispiel 1
$f(x) = x^3 -6x^2 +20$
$f'(x) = 3x^2 -12x$
$f''(x) = 6x -12$

$0 = 6x -12$
$x = 2$

$f'''(x) = 6 \neq 0 \implies W(2|4)$
$f'(2) = -12 = m_t$
$y = mx +n$
$4 = -12\cdot2 +n$
$n = 28$
$\implies t(x) = -12x +28$

#### Beispiel 2
$f(x) = e^x \cdot (2x^2 +2x)$
$f'(x) = e^x \cdot (2x^2 +2x) + e^x \cdot (4x + 2) = e^x \cdot (2x^2 +6x +2)$
$f''(x) = e^x \cdot (2x^2 +6x +2) + e^x \cdot (4x +6) = e^x \cdot (2x^2 +10x +8)$

$0 = e^x \cdot (2x^2 +10x +8)$
$0 = x^2 +5x +4$
$x_{1;2} = -\frac52 \pm \frac32$
$x_1 = -4$
$x_2 = -1$

$f'''(x) = e^x \cdot (2x^2 +10x +8) + e^x \cdot (4x +10) = e^x \cdot (2x^2 +14x +18)$

$f'''(-1) = e^{-1} \cdot (2 -14 +18) = 6e^{-1} \neq 0 \implies W_1(-1|0)$
$f(-1)= 0$
$f'(-1) = e^{-1} \cdot -2 = -2e^{-1} = m_{t_1}$
$0 = -2e^{-1} \cdot (-1) +n$
$n = -2e^{-1}$
$\implies t_1(x) = -2e^{-1} \cdot x - 2e^{-1}$

$f'''(-4) = e^{-4} \cdot (32 -56 +18) = -6e^{-4} \neq 0 \implies W_2(-4|24e^{-4})$
$f(-4) = 24e^{-4}$
$f'(-4) = e^{-4} \cdot (32 -24 +2) = 10e^{-4} = m_{t_2}$
$24e^{-4} = 10e^{-4}\cdot-4 +n$
$n = -64e^{-4}$
$t_2(x) = 10e^{-4} \cdot x +64e^{-4}$

#### Beispiel 3
$f(x) = -\frac14x^4 -x^3$
$f'(x) = -x^3 -3x^2$
$f''(x) = -3x^2 -6x$

$0 = -3x^2 -6x$
$0 = -3x(x +2)$
$x_1 = 0$
$x_2 = -2$

$f'''(x) = -6x -6$
$f'''(0) = -6 \neq 0 \implies W_1(0|0) \implies$ Sattelpunkt [[Mathe/2/2.4 Zusammenhänge zwischen den Graphen der Funktionen f, f' und f''/Zusammenhänge zwischen den Graphen der Funktionen f, f' und f''#Beispiel 3]]
$f'(0) = 0 = m_{t_1}$
$0 = 0 \cdot 0 +n$
$n = 0$
$t_1(x) = 0$

$f'''(-2) = 6 \neq 0 \implies W_2(-2|4)$
$f(-2) = 4$
$f'(-2) = 8 -12 = -4 = m_{t_2}$
$4 = -4\cdot-2 +n$
$n = -4$
$t_2(x) = -4x -4$

#### Beispiel A
$f(x) = x^6$

$f'(x) = 6x^5$
$0 = 6x^5$
$x = 0$

$f''(x) = 30x^4$
$f''(0) = 0 \implies$ ungeklärt

$f'''(x) = 120x^3$
$f'''(0) = 0 \implies$ ungeklärt

$f^{IV}(x) = 360x^2$
$f^{IV}(0) = 0 \implies$ ungeklärt

$f^V(x) = 720x$
$f^{V}(0) = 0 \implies$ ungeklärt

$f^{VI}(x) = 720$
$f^{VI}(0) = 720 \neq 0 \implies$ Extrempunkt
#### Beispiel B
$f(x) = x^5$

$f'(x) = 5x^4$
$0 = 5x^4$
$x = 0$
$f'(0) = 0 \implies$ ungeklärt

...

$f^V(x) = 120$
$f^V(0) = 120 \neq 0 \implies$ Wendepunkt

> [!note] #MatheDefinition 
> Wenn an einer verdächtigen stelle die 1., 2., 3. Ableitung $0$ ergeben untersucht man das verhalten höherer Ableitungen an dieser Stelle.
> 
> Man bestimmt die erste nicht verschwindende Ableitung.
> ($f^n(x) \neq 0$)
> 
> Ist $n$ gerade dann handelt es sich um eine Extremstelle. Beispiel A
> Ist $n$ ungerade dann handelt es sich um eine Sattelstelle. Beispiel B

