# 1. Einleitung
Algorithmisches Trading, auch als automatisierter Handel bekannt, hat sich in den letzten Jahre zu einer der dominierenden Methoden im Finanzsektor entwickelt.
Durch den Einsatz leistungsfähiger Computer und die zunehmende Vernetzung und Digitalisierung, ergibt sich die Möglichkeit es komplexe Handelsentscheidungen innerhalb kürzester Zeit zu treffen.
Der vollautomatisierte Handel ist in allen Investorengruppen von Institutionen über Fonds bis hin zu privaten Kleinanlegern verbreitet. Alle erhoffen sich durch den Einsatz Vorteile in den Märkten zu erzielen.

Das Ziel dieser Arbeit ist es, die Entwicklung einer eigenen algorithmischen Handelsstrategie zu untersuchen und die dafür notwendigen Schritte systematisch zu beschreiben.
Die Methodik der Arbeit umfasst die theoretischen Grundlagen des algorithmischen Tradings sowie die praktische Entwicklung einer eigenen Handelsstrategie mithilfe einer Programmiersprache. Der Aufbau gliedert sich wie folgt: Im zweiten Kapitel werden die Grundlagen und Entwicklung des algorithmischen Tradings erläutert. Das dritte Kapitel umfasst eine allgemeine Einführung in die Algorithmus Entwicklung. Im vierten Kapitel erfolgt die Auswahl der Indikatoren und Entwicklung eines eigenen Algorithmus. Kapitel fünf widmet sich dem Backtesting und Analyse der entwickelten Handelsstrategie, sowie Auswertung.

Mit dieser Arbeit soll ein fundierter Einblick in die Welt des algorithmischen Tradings gewährt werden und aufgezeigt werden, wie sich individuelle Handelsstrategien entwickeln lassen.

# 2. **Grundlagen des algorithmischen Tradings**
## 2.1 Definition
Algorithmisches Trading, auch als Algo Trading bezeichnet, umfasst die Anwendung von Software-Algorithmen für die vollautomatische Ausführung von Orders (Handelsaufträgen). Dabei lassen sich zwei große strategische Bereiche unterscheiden: einmal die Generierung von Orders (Buy Side-Algorithmen) und zum Anderen die Verwaltung dieser Aufträge (Sell Side-Algorithmen). Buy Side-Algorithmen überwachen ein Marktsegment mit dem Ziel bei einem profitablen Marktzustand einen Kaufauftrag für handelbare Papiere zu generieren. Dafür werden verschiedene Marktdaten fortlaufend analysiert. Sell Side-Algorithmen verwalten handelbare Papiere, das heißt beim Erreichen vorgegebener Parameter werden Kauf- oder Verkaufsaktionen durchgeführt. 
[[Belegarbeit#source_1]]

## 2.2 Entwicklung
Das Konzept des automatisierten Handelssystems wurde erstmals 1949 von Richard Donchian, einem amerikanischen Trader, angewendet. Zum damaligen Zeitpunkt musste die Ausführung festgeschriebener Regeln für das Kaufen und Verkaufen seiner Ressourcen noch manuell durch seine Angestellten verrichtet werden.
Mit der Entwicklung des Computers entstand auch die erste elektronische Handelsplattform die Anfang der 1980er von Thomas Peterffy eingeführt wurde. Er gründete das Unternehmen "Interactive Brokers".
Vollautomatisches Algorithmisches Trading zeigte sich in den 1990er Jahren zu ersten Mal. Die Entwicklung moderner leistungsfähiger Computer ermöglicht die Verbreitung von Algorithmischen Trading und ist somit kostengünstig bis hin zum Kleinanleger Bereich. Diese Art von automatisiertem Handel entwickelte sich aus der Idee Handelsentscheidungen schnell, ohne Emotionen und anderen Einflüssen die Menschen beeinträchtigen, zu treffen. Hochentwickelte Computer ermöglichen die Verarbeitung von wesentlich größeren Datenmengen und damit eine bessere und detaillierte Analyse der Marktdaten. Da der automatische Handel verschiedene Anlageklassen und Marktsegmente abdecken kann, lässt er eine schnellere Reaktion auf neue Marktchancen zu und damit breitere Portfolios, welche die Abhängigkeit von einzelnen Anlagepapieren reduzieren.
[[Belegarbeit#source_1]] [[Belegarbeit#source_2]] [[Belegarbeit#source_3]] [[Belegarbeit#source_4]]

//TODO: more

## 2.3 Wirtschaftliche Bedeutung und Markanteil
"Etwa 60-75 Prozent des gesamten Handelsvolumens auf dem US-amerikanischen Aktienmarkt, den europäischen Finanzmärkten und den wichtigsten asiatischen Kapitalmärkten werden laut Select USA im Jahr 2018 durch algorithmischen Handel generiert. Das gesamte Handelsvolumen des algorithmischen Handels in Schwellenländern wie Indien wird jedoch auf rund 40 Prozent geschätzt." [[Belegarbeit#source_5]]
Quantified Strategies, von der diese Aussage stammt, ist nur eine der vielen Online Plattformen die unter anderem Handelsstrategien zur Verfügung stellen und Märkte analysieren. Die Aussage verdeutlicht wie bedeutend das Algorithmische Trading für den internationalen Handel geworden ist.
Eine andere Analyse Plattform von Goldman Sachs veröffentlichte 2017 die in Abbildung 1 dargestellte Entwicklung des Markanteils von Algorithmischen Trading anhand der Auftrags-Klassen. Dort erkennt sich das enorme Wachstum des vollautomatischen Handels.
![[bilder/Market Share of Algo Trading.png]]
_Quelle: Goldman Sachs, Aite Group_

## 2.4 Grundlage Candles
Eine Candle (Kerze) repräsentiert die Preisentwicklung in einem definierten Zeitraum. Es gibt steigende und fallende Candles. Abbildung 2 zeigt die Informationen einer Candle.
![[Candle.png]]
Der Zeitraum den eine Candle umfasst ist frei wählbar. Der Zeitraum in dem die Handelswerte zu einer Candle zusammengefasst werden, wird als Intervall bezeichnet.

# 3. **Entwicklung einer eigenen Handelsstrategie**
## 3.1 Auswahl
Die Entwicklung einer Handelsstrategie kann in fünf Schritte geteilt werden. (more???) (simplifyed)

idk:
Einen eigenen Algorithmus zu entwickeln ist nicht so einfach ohne Vorwissen in anderen Themen wie Programmieren und das verstehen des Marktes und des Handelsobjektes welches man sich aussucht.
### 3.1.1 Handelsobjekt
Als erstens wird das Handelsobjekt festgelegt, wie etwa Aktien, Rohstoffe, Forex oder Indizes. Jedes Handelsobjekt hat verschiedene Vor- und Nachteile und es eigenen sich nicht alle Strategien für jedes Handelsobjekt. (examples???)
### 3.1.2 Kategorie
[[Belegarbeit#source_6]]
Folgend sollte eine Handelskategorie festgelegt werden. Hier stehen viele zur Wahl, am häufigsten sind: Day-, Positions-, Swing-, Trend-Trading und Scalping.
Day-Trading das Traden am Tag und das Schließen von Trades bevor der Marktschließung. Durch das klassische Verhalten werden Risiken vermieden, die zum Beispiel durch das nicht Beobachten des Objektes auftreten. Das verkleinert die Verluste und vermeidet zusätzliche Kosten.
Position-Trading basiert darauf über einen längeren Zeitraum eine offene Position zu unterhalten. Dies häufig über Wochen, Monate oder Jahre. Das "große" Zeit­fens­ter macht die Strategie zu einer Langzeit-Strategie, im Gegensatz zum Day-Trading welche eine Kurzzeit-Strategie ist.
Swing-Trading dagegen ist eine Zusammensetzung von technischen Analysen und den sog. "Swings" in den Preisbewegungen eines Handelsobjekts. "Ein 'Swing High' tritt auf, wenn sich der Kurs nach oben bewegt, ein 'Swing Low' bezeichnet hingegen einen Kursrückgang." ([[Belegarbeit#source_6]], Abs. Swing-Trading)???. Das Ziel der Strategie ist es Profit durch den Verkauf beim Kurshoch zu erzielen und durch Käufe beim Kurstief.
Dagegen ist das Ziel des Trend-Tradings eine Trendänderung zu identifizieren. Passend zu diesem Ziel entwickeln Trader eine Liste mit Bedingungen für das Öffnen und eine für das Schließen eines Trades. Somit ist der Zeitraum für einen offenen Trade in dieser Strategie irrelevant.
Im Gegenzug ist Scalping eine Strategie die auf dem Momentum von Preisbewegungen aufbaut. Was sie zu einer sehr kurzzeitig haltenden Strategie macht. Hier werden Position meist nur wenige Minuten oder sogar Sekunden gehaltenen. Trader die diese Strategie benutzen werden auch als Scalper bezeichnet.
(more to each???)
### 3.1.3 Indikatoren
Nach dem jetzt das Handelsobjekt und die Strategie-Kategorie festgelegt worden sind, können die Indikatoren rausgesucht werden, welche die gewünschten Ereignisse identifizieren. Hier gibt es praktisch unendlich viele verschiedene. Die richtige Balance und Kombination zu finden, könnte als eine unmögliche Aufgabe beschrieben werden. Durch dieses Phänomen ist es wichtig einen Toleranzbereich festzulegen, in welchem sich die identifizierten Ereignisse aufhalten. Einer der bekanntesten und meist genutzten ist der "EMA 200", "EMA" steht hier für Exponential Moving Average und "200" für 200 Candles als Datenmenge. Was der "EMA 200" zeigt ist der Trend eines Preiskurses, in diesem fall ein langzeitiger Trend. Es können auch kürzere Trends bestimmt werden in dem der Zeitraum des Indikators verkürzt wird, zum Beispiel 30 Tage um einen mittelzeitigen Trend zu identifizieren. [[Belegarbeit#source_7]] (idk???)
### 3.1.4 Implementierung
Der nächste Schritt ist die Implementierung der Indikatoren. Es müssen also eine Programmiersprache und Programme ausgewählt werden in denen die Indikatoren dann geschrieben werden um den Vorgang vollautomatisch zu machen sowie die Möglichkeit Kauf- und Verkaufsaufträge stellen zu können. Um ein Beispiel zu nennen könnte man Python als Programmiersprache und Metatrader5 als Program benutzten. Für Metatrader5 existiert eine Bibliothek in Python was das interagieren wesentlich vereinfacht. [[Belegarbeit#source_9]] (more!???)
### 3.1.5 Backtesting und Analyse
Als letztes ist das Backtesting und die Analyse sowie Fein-Tuning von den Indikatoren. Dies ist der Schritt der meist die einzelne Parameter der Indikatoren verändert, wie bei EMA 200 könnte sich herausstellen das der EMA 100 besser geeignet ist oder umgekehrt. Es werden also die Parameter geändert um die Empfindlichkeit der Indikatoren anzupassen damit sie in den gewünschten Toleranzbereich kommen. Und nicht zu früh oder zu spät die ausgewählten Ereignisse identifizieren um den Profit zu erhöhen und nicht vielleicht sogar eine verlierenden Algorithmus zu haben der über längere Zeit Verluste macht. (more!???)
## 3.2 eigener Algorithmus
### 3.2.1 Handelsobjekt
Ich benutzte für meine Arbeit, den Handelswert "FXOPEN:XAUUSD". Es ist ein beim Broker FXOPEN gehandelter Goldwert auf der Basis von US-Dollar. Es handelt sich dabei um ein Waren CFD von Gold. CFD-Trading ist das Spekulieren von Preisbewegungen eines Handelsobjektes, somit besitzt man nicht das Handelsobjekt selbst und ist nur den Preisbewegungen ausgesetzt. Ein Vorteil ist die Flexibilität der CFDs, da Profite können durch Fallen und Steigen des Preises erzielt werden.
[[Belegarbeit#source_10]]
### 3.2.2 Kategorie
Ich habe mich für Trend-Trading entschieden im 30 Minuten Intervall, da ich zur Zeit in diesem Bereich über die größte Erfahrung verfüge.
### 3.2.3 Indikatoren
#### 3.2.3.1 EMA
Wie schon beschrieben handelt es sich hier um den Exponential Moving Average. Welche Candle Menge hier am besten passt ist wird sich im Backtesting herausstellen. Ich werde hier einen größeren Wert verwenden um weniger reaktiv auf Ausbrüche zu sein. 
#### 3.2.3.2 Relativ Strength Index (RSI)
Der RSI ist ein Momentum-Indikator. Er beschreibt die Geschwindigkeit der Änderung des Preises.
![[RSI.png]]
[[Belegarbeit#source_11]]
Der Indikator kann Werte zwischen 0 und 100 annehmen. Dabei sind große Werte Anzeichen dafür das das Objekt stark gekauft wird und Werte kleiner 30 das es stark verkauft wird, wird auch als Überkauf und Überverkauf bezeichnet. Welche Candle Menge genau am besten wird sich auch hier wieder im Backtesting zeigen, da ich allerdings einen mehr reaktiven RSI haben möchte wird es sehr wahrscheinlich nicht über 20 gehen. 
### 3.2.4 Implementierung
Die Implementierung werde ich in PineScript ausführen, um das Backtesting zu vereinfachen. PineScript ist eine Programmiersprache die von der Charting-Plattform TradingView entwickelt wurde und dort direkt ausführbar ist. Da sie auf die Erstellung von Indikatoren und Algorithmen spezialisiert ist, sind somit auch schon alle notwendigen Funktionen um Handel zu betreiben vorhanden.
#### 3.2.4.1 EMA
Die Formel für den Exponential Moving Average ist:
$EMA_{n} = \frac{Wichtung}{1+Länge} \cdot Preis_{n} + EMA_{n-1}\cdot(1-\frac{Wichtung}{1+Länge})$
wobei "Wichtung" beschreibt wie stark die neuesten Werte in die Berechnung eingehen. Und "Länge" die Anzahl der verwendeten Candles ist.
[[Belegarbeit#source_12]]
##### Implementiert
```PineScript
source_ema = input.source(close, "source", group = "EMA")
length_ema = input.int(100, "length", group = "EMA")
ema_value = ta.ema(source_ema, length_ema)
plot(ema_value, title = "ema_value", color = color.blue)
```
Da TradingView eine eingebaute Funktion für den EMA hat, kann ich mir Zeit und Arbeit sparen. Wenn der EMA unter den Preis fällt, dann möchte ich ein Kaufsignal. Und ein Verkaufsignal wenn der EMA über den Preis steigt.
```PineScript
long_ema = ta.crossunder(ema_value, source_ema)
short_ema = ta.crossover(ema_value, source_ema)
```
#### 3.2.4.2 RSI
Der Relativ Strength Index wird in vier Stufen gebildet. Grundlage sind wählbare Eckdaten der Candle (Öffnungs-, Höchster-, Niedrigster-, Schließungspreis)
a) Änderung zum vorherigen Preis.
$Änderung_{n} = Preis_{n} - Preis_{n -1}$
b) Feststellen ob Gewinn oder Verlust
$Gewinn_{n} = max\{Änderung_{n};0\}$
$Verlust_n = -(min\{Änderung_n;0\})$
c) Mittelwert von Gewinn und Verlust
$RMA_{Gewinn_{n}} = \frac{1}{Länge} \cdot Gewinn_{n} + RMA_{Gewinn_{n-1}}\cdot(1-\frac{1}{Länge})$
$RMA_{Verlust_{n}} = \frac{1}{Länge} \cdot Verlust_{n} + RMA_{Verlust_{n-1}}\cdot(1-\frac{1}{Länge})$
d) relative Stärke und index
$rs = \frac{RMA_{Gewinn_{n}}}{RMA_{Verlust_{n}}}$
$index = 100 - \left( \frac{100}{1+rs} \right)$
[[Belegarbeit#source_13]]
##### Implementiert
```PineScript
source_rsi = input.source(close, "source", group = "RSI")
length_rsi = input.int(32, "length", group = "RSI")
// lay rsi over price graph and adjust to lay 50 on the price
rsi_value = ta.rsi(source_rsi, length_rsi) - 50 + source_rsi
plot(rsi_value, title = "rsi_value", color = color.purple)
```
Wie beim EMA hat TradingView auch für den RSI eine eingebaute Funktion. Wenn der RSI über den Preis steigen, dann möchte ich ein Kaufsignal und im Gegenteil ein Verkaufsignal.
```PineScript
long_rsi = ta.crossover(rsi_value, source_rsi)
short_rsi = ta.crossunder(rsi_value, source_rsi)
```

#### 3.2.4.3 Verbinden der Indikatoren
Wenn sich beide Indikatoren einig sind, wird die jeweilige Handelsaktion durchgeführt.
```PineScript
if long_ema and long_rsi and time_cond
    strategy.close_all()
    strategy.entry("long", strategy.long)

if short_ema and short_rsi and time_cond
    strategy.close_all()
    strategy.entry("short", strategy.short)
```
Die Variable "time_cond" ist nur da, um ein Zeitfenster festzulegen. Somit können die Statistiken von dem Strategy Tester direkt benutzt werden, ohne aufwendige Umrechnungen.
```PineScript
start_date = input.time(timestamp("2024-11-15T00:00:00"), group = "time window")
end_date = input.time(timestamp("2024-11-30T00:00:00"), group = "time window")
time_cond = time >= start_date and time <= end_date
```
### 3.2.5 Backtesting und Analyse
Der Algo ist eingestellt mit einem Startvermögen von 10'000 USD (Papiergeld) und pro Kaufaktion mit 80% seines Gesamtvermögens zu handeln. Ich betrachte einen relativ kurzen aber Informationsreichen Zeitraum, ab dem 15. November 2024 bis zum 30. November 2024.

![[chart_raw.png]]

Im dem folgenden Bild können wir sehen was die Indikatoren errechnen und wo der Algo Handel betreibt. Dies wurde nach ein bisschen rumprobieren wie vorher erwähnt, eingestellt mit dem EMA einer Candle Länge von 100 und dem Schließungspreis und dem RSI einer Candle Länge von 32 und dem Schließungspreis.

![[chart_all.png]]

Der erste Trade ist genau wo rauf diese Strategie abzielt. Er geht vom 18. November 2024 00:30Uhr mit einem Preis von 2'573,99 USD bis zum 25. November 2024 04:30Uhr mit einem Preis von 2'671,38 USD, erzielt rund 300 USD mit einer Handelsgröße von 3,1 Einheiten. Dabei hat er "nur" einen maximalem Drawdown (der höchst mögliche Verlust) von 12,93 USD, diese ist gleich nach dem Einstieg in den Trade und somit absolut erwartet. Der maximale Run-up (der höchst mögliche Profit) liegt hier bei rund 456,82 USD und somit zwar 50% mehr als der Profit, allerdings auch nur da unser EMA 100 zu träge ist um ein Verkaufssignal eher zu geben. Was allerdings den Trade auch beschützt hat am 20. November 2024, wäre ohne diese Trägheit ein Verkaufssignal gekommen und wir hätten den ganzen Profit danach verloren. Im ganzen ist es genau der Trade denn ich versucht habe mit dieser Kombination zu finden, den Trendveränderung am 18. November 2024 bis zum nächsten Wechsel am 25. November 2024.

![[1_Trade_Graph.png]]

Später allerdings sehen wir das Problem das sich mit der Trägheit von dem EMA 100 mit zieht. Da der EMA praktisch fast Stabil bleibt und sich mit dem Preis angleicht, zusammen mit reaktiven RSI entstehen hier viele Handelsaktionen welche zu Verlusten führen, wenn auch nur kleinen.

![[P_Trade_Graph.png]]

Insgesamt gehen hier 51,88 USD verloren, in 4 Trades. 

# 6. Zusammenfassung
Der in der vorliegenden Arbeit vorgestellte eigene Algorithmus für Trend-Trading ist nur ein kleines Beispiel von unendlich vielen Möglichkeiten von Indikatorkombinationen. Er soll den prinzipielle Vorgehensweise beim Algorithmischen Trading verdeutlichen. Über das gesamte Zeitfenster von 15 Tagen platziert mein Algorithmus 5 Trades. Dabei erwirtschaftet er 250.03 USD Profit und hat einen "Profit Factor", Gewinn pro ein Einheit Verlust, von 5,819. Was heißt das pro 1 USD Verlust rund 6 USD Gewinn erzielt hat. Zudem mit nur einem Profitable Trade Prozentanteil von 20% und einem maximalem Drawdown von 246,13 USD.
