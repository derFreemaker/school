# Generator: Außenplomaschine
Berechnen sie das Maximum der Wechselspannung eines Generators. Bei dem sich 80 Leiterstäbe von 40cm Länge am Umfang einen Trommelförmigen Rotors von 30cm Durchmesser in einem Feld von 0,6 Tesla mit einer Drehzahl von 750rpm.

> [!note] Variables
> $l = 40cm$
> $d = 30cm$
> $N = 40$ ... Windungszahl

- Maximum (Scheitelwert) der Induktionsspannung
  $\sin(\omega t) = 1$
- Fläche einer Leiterdichte
  $A = l\cdot d$
- Winkelgeschwindigkeit
  $\omega = 2\pi f=2\pi\cdot \frac{n}{60s}$ mit f ... Drehfrequenz

Induktionsspannung
$U_i = N\cdot B\cdot A\cdot \omega\cdot \sin(\omega t)$

Scheitelwert
$Û_{i} = N\cdot B\cdot l\cdot d\cdot 2\pi\cdot \frac{n}{60}\cdot1$

$Û_{i} \approx 226V$

# 1
Leistung $P=U\cdot I$
Stromstärke $I=\frac{P}{U}$ mit $P=500MW$
$I_{1} = 2'173'913A$ für $U_{1} = 230V$
$I_{2} = 25'000A$ für $U_{2} = 20kV$
$I_{3} = 1'315A$ für $U_{3} = 380kV$

# 2

## a
verlustfreier Betrieb -> Kurzschluss
$\frac{I_{1}}{I_{2}} = \frac{N_{2}}{N_{1}} \implies I_{1}=I_{2}\cdot \frac{N_{2}}{N_{1}}$
$I_{1} = 2A$

10A-Sicherung ist ausreichend.

## b
Leerlauf
$\frac{U_{1}}{U_{2}} = \frac{N_{1}}{N_{2}} \implies U_{2}=U_{1}\cdot \frac{N_{2}}{N_{1}}$
$U_{2} = 2,2V$

ungefährlich

# 3

## a
Leerlauf
$\frac{U_{1}}{U_{2}} = \frac{N_{1}}{N_{2}} \implies U_{2}=U_{1}\cdot \frac{N_{2}}{N_{1}}$
$U_{2} = 4.4kV$

## b
Idealfall -> Kurzschluss
$\frac{I_{1}}{I_{2}} = \frac{N_{2}}{N_{1}} \implies I_{2}=I_{1}\cdot \frac{N_{1}}{N_{2}}$
$I_{2} = 0.3A$

Real fall
$I_{2}\cdot\eta$
$0.3A \cdot92\%= 0.276A$
