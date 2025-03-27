
> [!def] #MatheDefinition 1
> Eine Stelle $x_{\max} \epsilon D_f$ heißt **relative Maximum** der Funktion $f$ genau dann,
> wenn es eine Umgebung $U \subseteq D_f$ von $x_\max$ derart gibt,
> dass für alle $x \in U$ gilt $f(x) \leq f(x_\max)$.
> Der Funktionswert $f(x_\max)$ heißt **relatives Maximum** der Funktion $f$.
> Der Punkt $H(x_\max|f(x_\max))$ heißt **relativer Maximumpunkt** oder **Hochpunkt** der Funktion $f$.

> [!def] #MatheDefinition 2
> Eine Stelle $x_{\max} \epsilon D_f$ heißt **relative Minimum** der Funktion $f$
> genau dann, wenn es eine Umgebung $U \subseteq D_f$ von $x_\max$ derart gibt,
> dass für alle $x \in U$ gilt $f(x) \geq f(x_\max)$.
> Der Funktionswert $f(x_\max)$ heißt **relatives Minimum** der Funktion $f$.
> Der Punkt $T(x_\max|f(x_\max))$ heißt **relativer Minimumpunkt** oder **Tiefpunkt** der Funktion $f$.

> [!def] #MatheDefinition 3
> Eine Stelle $x_E \in D_f$ heißt **relative Extremstelle** der Funktion $f$
> genau dann, wenn es sich um eine **relative Maximumstelle** oder eine **relative Minimumstelle** handelt.
> Der Funktionswert $f(x_E)$ heißt **relatives Extremum** der Funktion $f$.
> Der Punkt $E(x_E|f(x_E))$ heißt **relativer Extrempunkt** der Funktion $f$.

> [!def] #MatheDefinition 4
> Ein Punkt $P$ heißt **Sattelpunkt** einer Funktion $f$
> genau dann, wenn:
> - der Graph von $f$ im Punkt $P$ eine **waagerechte Tangente** besitzt.
> - der Punkt $P$ kein **relativer Extrempunkt** vom Graphen von $f$ ist.

## Zusammenhang 1
Die **Extremstellen** und **Sattelstellen** von $f$ sind die **Nullstellen** von $f'$.

## Zusammenhang 2
Der Verlauf des Graphen von $f'$ beschreibt das **Monotonieverhalten** des Graphen von $f$.

| Eine Funktion $f$ ist<br>in einem Intervall $I \subseteq D_f$ | wenn für alle $x \in I$ gilt |
| ------------------------------------------------------------- | ---------------------------- |
| monoton steigend                                              | $f'(x) \geq 0$               |
| streng monoton steigend                                       | $f'(x) > 0$                  |
| monoton fallend                                               | $f'(x) \leq 0$               |
| string monoton fallend                                        | $f'(x) < 0$                  |

## Zusammenhang 3
Die **Extremstellen** und **Sattelstellen** von $f'$ sind die **Nullstellen** von $f''$.

## Zusammenhang 4
Der Verlauf des Graphen von $f''$ beschreibt das **Monotonieverhalten** des Graphen von $f'$.


> [!def] #MatheDefinition 5
> Eine Stelle $x_W$ heißt **Wendestelle** der Funktion $f$ wenn die Ableitungsfunktion $f'$ an dieser Stelle ein **relatives Extremum** besitzt.
> Der Punkt $W(x_W|f(x_W))$ heißt **Wendepunkt** des Graphen von $f$.
> Die Tangente an den Graphen von $f$ im Punkt $W$ heißt **Wendetangente**.
> > [!TIP] Spezialfall
> > Sattelpunkt =
> > - Horizontalwendepunkt
> > - Wendepunkt mit horizontaler Wendetangente


> [!def] #MatheDefinition 5 Alternative
> Eine Stelle $x_W$ heißt **Wendestelle** des Graphen von $f$,
> wenn der Graph von $f$ beim durchlaufen dieser Stelle von einer Linkskrümmung in eine Rechtskrümmung übergeht oder umgekehrt.
> Der Punkt $W(x_W|f(x_W))$ heißt **Wendepunkt** des Graphen von $f$.

## Zusammenhang 5
Die **Wendestellen** von $f$ sind die **Nullstellen** von $f''$

## Zusammenhang 6
Der Verlauf des Graphen von $f''$ beschreibt das Krümmungsverhalten des Graphen von $f$.
$f''(x) < 0 \implies \text{rechtsgekrümmt}$
$f''(x) > 0 \implies \text{linksgekrümmt}$

# Berechnung relativer Extrempunkte

> [!tip] Bedingungen
> ###### Notwendig:
>   $f'(x) = 0$
> ###### Hinreichend:
>   $f''(x_E) \neq 0$
>   $f''(x_E) > 0$ -> linksgekrümmt => Min
>   $f''(x_E) < 0$ -> rechtsgekrümmt => Max

## Vorgehensweise
1. Mann setzt $f'(x) = 0$ und bestimmt alle stellen mit waagerechter Tangente.
2. Mann setzt die verdächtigen stellen in $f''(x)$ ein und prüft ob es sich tatsächlich um Extremstellen handelt. Gleichzeitig erhält man die Art des Extremums.
3. Mann setzt die Extremstelle in $f(x)$ und ermittelt die fehlenden Funktionswerte.

### Bespiel 1
$f(x) = x^3 -2x^2 -6$
$f'(x) = 3x^2 -4x$
$f''(x) = 6x -4$

$0 = 3x^2 -4x$
$0 = x(3x -4)$
$x_1 = 0; x_2 = \frac43$

$f''(x_1) = -4 \implies Max(0|-6)$
$f''(x_2) = 4 \implies Min(\frac43|-\frac{194}{27})$

### Beispiel 2
$f(x) = x^4 -8x^2$
$f'(x) = 4x^3 -16x$
$f''(x) = 12x^2 -16$

$0 = 4x^3 -16x$
$0 = 4x(x^2 -4)$
$x_1 = 0; x_{2|3} = \pm2$

$f''(0) = -16 < 0\implies Max(0|0)$
$f''(2) = 32 > 0 \implies Min(2|-16)$
$f''(-2) = 32 > 0 \implies Min(-2|-16)$

### Beispiel 3
$f(x) = -\frac14x^4 -x^3$
$f'(x) = -x^3 -3x^2$
$f''(x) = -3x^2 -6x$

$0 = -x^3-3x^2$
$0 = -x^2(x + 3)$
$x_1 = 0; x_2 = -3$

$f''(0) = 0 \implies$ bleibt vorläufig ungeklärt
$f''(-3) = -9 \implies Max(-3|\frac{27}4)$

## Übung
1. $f(x) = \frac13x^3-\frac12x^2-6x$
$f'(x) = x^2 -x -6$

$0 = x^2 -x -6$
$x_{1;2} = -\frac12 \pm 2.5$
$x_1 = -3$
$x_2 = 2$

TODO: finish

2. $f(x) = \frac38x^4 +\frac92x^2$
$f'(x) = \frac{3}{2}x^3 +9x$

$0 = x(\frac{3}{2}x^2 + 9)$
$x_1 = 0$

$f''(x) = \frac92x^2 + 9$
$f''(0) = 9 > 0 \implies Min(0|0)$

3. $f(x) = \frac1x-\frac1{x^2} = x^{-1} - x^{-2}$
$f'(x) = x^{-2} +2x^{-3}$

$0 = x^{-2} +2x^{-3}$
$x_1 = 0$

$f''(x) = x^{-2} +x^{-3}$
$f''(0) = 0 = 0 \implies$ bleibt vorläufig ungeklärt

 4. Arbeitsblatt
$P(N) = -\frac{N^3}{15} +\frac{4N^2}{5} +4N = -N^3 \cdot 15^{-1} + 4N^2 \cdot 5^{-1} + 4N$
$P'(N) = -\frac{N^2}{5} +\frac{8N}{5} +4 = -3N^2\cdot15^{-1} +8N\cdot5^{-1} +4$

$0 = -N^2 +8N +20$ $|\cdot(-1)$
$0 = N^2 -8N - 20$
$x_{1;2} = -\frac{p}{2} \pm \sqrt{(\frac{p}{2})^2 -q}$
$x_{1;2} = 4 \pm 6$
$x_1 = -2$
$x_2 = 10$

$P''(N) = -\frac{2N}{5} +\frac{8}{5}$
$P''(10) = -\frac{12}{5} < 0 \implies Max(10|P(10))$

Zusatz: $f(x) = \frac{3x^2 -8x}{(x-2)^2}$
