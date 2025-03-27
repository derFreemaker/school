# 1
## a
Blindwiderstand
$X_{L} = 2\pi\cdot10\cdot10^3Hz\cdot5000\cdot10^{-6}H$
$X_{L} \approx 314.16\ohm$

## b
Gesamtwiderstand
(Scheinwiderstand)
$Z=\sqrt{ R^2+X_{L}^2 }$
$Z\approx 314.16$

## c
Phasenverschiebung
$\tan\varphi = \frac{X_{L}}{R}$
$\varphi = 89.78°$

Wirkleistung
$P=U\cdot I\cdot \cos \varphi$
$P\approx 479mW$

# 2
Induktionsspannung
$U_{i}= N\cdot B\cdot A\cdot \omega\cdot \sin (\omega t)$
mit $\sin(\omega t) = 1$ für Scheitelwert
mit $\omega = 2\pi\cdot f=2\pi\cdot \frac{n}{60}$

$U_{i} = N\cdot B\cdot A\cdot2\pi\cdot \frac{n}{60}$

Flussdichte
$B=\frac{60\cdot U_{i}}{N\cdot A\cdot2\pi\cdot n}$
$B= \frac{60\cdot100}{1000\cdot0.1\cdot2\pi\cdot6000}$
$B\approx 16mT$

Einheit: $1\frac{s\cdot V}{m^2} = 1\frac{s\cdot V\cdot A}{m^2\cdot A} = 1\frac{N\cdot m}{m^2\cdot A} = 1\frac{N}{m\cdot A} = 1T$

# 3
Wirkleistung $P=U\cdot I\cdot \cos \varphi = S\cdot \cos \varphi$
Scheinleistung $S =U\cdot I =\frac{P}{\cos \varphi}$
$S =6k\text{ }VA$

Blindleistung $Q= \sqrt{ S^2-P^2 }$
$Q =3.75k\text{ }var$

Stromaufnahme
$I=\frac{S}{U}$
$I=\frac{6'000VA}{220V}$
$I= 28.41A$

Wirkungsgrad $Wirkungsgrad_{mech}= \frac{P_{mech}}{P_{el}}$
$P_{mech} = Wirkungsgrad_{mech}\cdot P_{el}$ mit $P_{el}=5kW$
$P_{mech} = 4.25kW$

# 4
## a

Wirkleistung
$P=2\cdot260W=520W$
$P=U\cdot I\cdot \cos \varphi$
$P=S\cdot \cos \varphi$

Scheinleistung
$S = \frac{P}{\cos \varphi}$
$S = \frac{520}{\cos0.79} \approx 658 \text{VA}$

> [!note]
> Die Angabe eines Leistungsfaktors $\cos \varphi$ bezieht sich immer auf die Sekundärseite (OUT) des Transformators.

## b

Wirkungsgrad
$\eta=\frac{P_{2}}{P_{1}}=\frac{S_{2}}{S_{1}}=\frac{\text{OUT}}{\text{IN}}$
$\eta=\frac{S_{2}}{S_{1}}$
$S_{1} = \frac{658}{0.91} = 723\text{VA}$

$S_{1} = U_{1}\cdot I_{1}$
$I_{1} = \frac{S_{1}}{U_{1}}$
$I_{1}= \frac{723}{230} = 3.14A$
