### Thema: **"Algorithmisches Trading: Entwicklung einer eigenen Handelsstrategie"**

### Gliederung:
1. **Einleitung (1 Seite)**
    - Vorstellung des Themas und seiner Relevanz.
    - Zielsetzung und Struktur der Arbeit.
2. **Grundlagen des algorithmischen Tradings (2 Seiten)**
    - Definition und Entwicklung des algorithmischen Tradings.
    - Überblick über wirtschaftliche Bedeutung und Marktanteil.
3. **Entwicklung einer eigenen Handelsstrategie (3 Seiten)**
    - Auswahl und Kombination von technischen Indikatoren. (EMA 200 & RSI)
    - Beschreibung der Kauf- und Verkaufsregeln (Anwendung).
    - Implementierung in einer geeigneten Softwareumgebung.
4. **Backtesting und Analyse (2 Seiten)**
    - Durchführung von Backtests mit historischen Daten.
    - Auswertung der Ergebnisse hinsichtlich Rentabilität und Risiko.
    - Diskussion der Ergebnisse im Kontext der rechtlichen und wirtschaftlichen Implikationen.
5. **Fazit und Ausblick (1 Seite)**
    - Zusammenfassung der zentralen Erkenntnisse.
    - Einschätzung der Chancen und Risiken des algorithmischen Tradings.
6. Verzeichnisse

# 3. Entwicklung
- Auswahl
	- Was traden wir?
	- Kategorie (Bilder von Webseite nutzen)
		- Day-Trading
		- Positions-Trading
		- Swing-Trading
		- Trend-Trading
		- Scalping
	- Indikatoren
		- EMA 200
		- RSI
		- (Twin Range Filter)
	- Implementierung
	- Optimierung durch Backtesting und Analyse

- Erklärung und Zusammenstellung jedes Indikators
	- EMA 20-50
		- siehe oben
	- RSI mit EMA 50
		- summen der positiven und negativen Bewegungen
		  $sum_{up}(t) = \sum\limits_{i=1}^n{max\{P(t - i +1) - P(t - i);0\})}$
		  $sum_{down}(t) = -\sum\limits_{i=1}^n{min\{P(t - i +1) - P(t - i);0\})}$
		- Mittelwert
		  $avg_{up} = \frac{sum_{up}}{n}$
		  $avg_{down} = \frac{sum_{down}}{n}$
		- RSI
		  $RSI = \frac{avg_{up}}{avg_{up}+avg_{down}}$
	- (Twin Range Filter)
		//TODO: untangle this mess
		```PineScript
		source = input(defval=close, title='Source')
		showsignals = input(title='Show Buy/Sell Signals ?', defval=true)
		per1 = input.int(defval=27, minval=1, title='Fast period')
		mult1 = input.float(defval=1.6, minval=0.1, title='Fast range')
		per2 = input.int(defval=55, minval=1, title='Slow period')
		mult2 = input.float(defval=2, minval=0.1, title='Slow range')
		smoothrng(x, t, m) =>
			wper = t * 2 - 1
			avrng = ta.ema(math.abs(x - x[1]), t)
			smoothrng = ta.ema(avrng, wper) * m
			smoothrng
		smrng1 = smoothrng(source, per1, mult1)
		smrng2 = smoothrng(source, per2, mult2)
		smrng = (smrng1 + smrng2) / 2
		rngfilt(x, r) =>
			rngfilt = x
			rngfilt := x > nz(rngfilt[1]) ? x - r < nz(rngfilt[1]) ? nz(rngfilt[1]) : x - r : x + r > nz(rngfilt[1]) ? nz(rngfilt[1]) : x + r
			rngfilt
		filt = rngfilt(source, smrng)
		upward = 0.0
		upward := filt > filt[1] ? nz(upward[1]) + 1 : filt < filt[1] ? 0 : nz(upward[1])
		downward = 0.0
		downward := filt < filt[1] ? nz(downward[1]) + 1 : filt > filt[1] ? 0 : nz(downward[1])
		STR = filt + smrng
		STS = filt - smrng
		FUB = 0.0
		FUB := STR < nz(FUB[1]) or close[1] > nz(FUB[1]) ? STR : nz(FUB[1])
		FLB = 0.0
		FLB := STS > nz(FLB[1]) or close[1] < nz(FLB[1]) ? STS : nz(FLB[1])
		TRF = 0.0
		TRF := nz(TRF[1]) == FUB[1] and close <= FUB ? FUB : nz(TRF[1]) == FUB[1] and close >= FUB ? FLB : nz(TRF[1]) == FLB[1] and close >= FLB ? FLB : nz(TRF[1]) == FLB[1] and close <= FLB ? FUB : FUB
		long = ta.crossover(close, TRF)
		short = ta.crossunder(close, TRF)
		```
	- Software:
		- PineScript for Backtesting in TradingView

# 6. Verzeichnisse
## Glossar
- Trader
  Ein Trader ist eine Händler/Person die mit dem Markt, meist digital, interagiert.
- Indizes
  Indizes sind eine Gruppe von Aktien, Krypto und anderen (z.B.: S&P 500).

# Quellen
### source_1
- Autor: Prof. Dr. Dennis Kundisch
- Title: Algorithmic Trading
- URL: https://www.gabler-banklexikon.de/definition/algorithmic-trading-70264
- Datum: 21.12.2024
### source_2
- Autor: Niklas Mueller
- Titel: Was ist ein Algo Trading? | Algorithmischer Handel erklärt
- URL: https://trading.de/lernen/algo-trading/
- Datum: 21.12.2024

### source_3
- Autor: Richard Donchian
- Titel: Donchian’s 5 and 20 day Moving Averages
- URL: https://www.chrisperruna.com/2007/09/24/donchians-5-and-20-day-moving-averages/
- Datum: 21.12.2024

### source_4
- Autor: Jacob Bunge
- Title: Interactive Brokers Founder, CEO To 'Gradually' Retire
- URL: https://www.wsj.com/articles/BL-DLB-37771
- Datum: 21.12.2024

## source_5
- Autor: Oddmund Groette
- Title: What Percentage of Trading Is Algorithmic? (Algo Trading Market Statistics)
- URL: https://www.quantifiedstrategies.com/what-percentage-of-trading-is-algorithmic/
- Datum: 22.12.2024
### source_6
- Autor: ???
- Title: Die Top-5-Handelsstrategien
- URL: https://www.ig.com/de/trading-strategien/die-top-5-handelsstrategien-190307
- Datum: 22.12.2024

### source_7
- Autor: ???
- Title: EMA 200 | Berechnung und Einsatz im Trading
- URL: https://tradistats.com/ema-200-berechnung-und-einsatz-im-trading/
- Datum: 28.12.2024

### source_8 (dead)
- URL: https://www.purple-trading.com/candlestick-patterns-in-trading-and-how-to-trade-them/
- Datum: 30.12.2024

### source_9
- Title: MetaTrader module for integration with Python
- URL: https://www.mql5.com/en/docs/python_metatrader5
- Datum: 30.12.2024

### source_10
- URL: https://www.ig.com/en/cfd-trading/what-is-cfd-trading-how-does-it-work
- Datum: 5.1.2025

### source_11
- URL: https://www.lynxbroker.de/app/uploads/2016/06/20160609-Momentum-indikatoren-Relative-Strength-Index-RSI-lynx-daytrading.png
- Datum: 5.1.2025

### source_12
- URL: https://de.tradingview.com/support/solutions/43000592270/#:~:text=Der%20%E2%80%9EExponential%20Moving%20Average%E2%80%9C%20ist,mit%201%20minus%20den%20Multiplikator
- Datum: 5.1.2025

### source_13
- URL: https://www.tradingview.com/support/solutions/43000502338-relative-strength-index-rsi/
- Datum: 5.1.2025
