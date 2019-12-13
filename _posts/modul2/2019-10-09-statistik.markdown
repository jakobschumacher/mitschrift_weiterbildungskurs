---
layout: post
title:  "Einführung in die Statistik"
date:   2019-10-09 08:00:00 +0100
categories: Modul-2
permalink: statistik/
autor: 202
vortrag:
  - 100919Arnold_Statistik1.pdf
  - 100919Arnold_Statistik2.pdf
---

* Statistik ist ein Werkzeug um Aussagen zu treffen

## Begriffe
* Population bestehen aus all denjenigen Objekten, über die man eine Aussage treffen möchte
* In Zufallsstichproben hat jedes Element die gleiche Chance ausgewäht zu werden
* Inferenz (Rückschluss) Aussage über die Population aufgrund einer Stichprobe. Verallgemeinerung
* Statistik gibt Werkzeuge, die es ermöglichen, das Risiko einer Falschaussage zu minimieren

|Einheit|Terminologie|Notation|
|---|---|---|
|Population| Menge aller relevanten Beobachtungseinheiten| Ausmaß: N, Parameter: mu|
|Stichprobe|(Zufalls-)Auswahl von Beobachtungseinheiten aus der Population|Ausmaß: n, Parameter x|
|Beobachtungseinheit|Kleinste Einheit der Beobachtung un Statistikanalyse||
|Zufallsvariable oder Wert|Merkmale der Beobachtungseinheiten|Zufallsvariable: X, individ. Wert: xi|

## Von der Idee zur Untersuchung
<div class="mermaid">
graph TD;
  a[Fragestellung]
  b[Planung]
  c[Datenerhebung]
  d[Datenauswertung]
  e[Interpretation]
  a-->b
  b-->c
  c-->d
  d-->e
  e-->a
</div>

## Berechnung einer Stichprobengröße
### Faustregel 1
* Zellbesetzung >5
* Folgendes muss erfüllt sein: n*(1-Stichprobenanteil in %) >5
* Beispiel: Wenn am Sonntag 
  - Variablen: Geschlecht (2 Kategorien), Alter (4 Kategorien), Schichtzugehörigkeit (3 Kategorien), Wahlbeteiligung (2 Kategorien). Insgesamt 48 Zellen
  - Es müssen also 5*48 = 240 Personen befragt werden
### Faustregel 2
* Festlegung einer Grenze (z.B. 5%)
* 1/Wurzel(n) 
* Beispiel: 1/Wurzel(1000) = 0,03 entspricht 3%

## Bevölkerungsstudien 
* Das RKI macht drei große Bevölkerungsstudien: GEDA, KIGGS, DEGS
* GEDA 1.0
  - N: Deutschsprachige Wohnbevölkerung in Privathaushalten ab 18 Jahren, die über einen Festnetzanschluss zu erreichen sind
  - Zusallstichprobe aus Nummern-pool aller öffentlich zugänglichen rufnummern (Gabler-Häder-Verfahren 1999)
  - Kontaktaufnahme der Haushalte und Auswahl der Zielperson nach der Last-Birthday-nethode
  - Merkmal und Ausprägung
    - z.B. Merkmal: Sozioökonomischer Status zugehörige Ausprägung wird durch drei Indikatoren gebildet (Bildungsstand, Berufsstatus, Einkommen). Aus den drei Indikatoren werden die Ausprägungen berechnet. 
* GEDA Daten sind [public use files](https://www.rki.de/DE/Content/Forsch/FDZ/informationen_datensaetze/info_datensaetze_node.html)  


## Skalenniveau

|Skala|Definition|Mögliche Aussagen|Beispiel|
|---|---|---|---|---|
|Nominal|Häufigkeiten|Äquivalenzrelation|Geschlecht, ICD-10|
|Ordinal|+Rangfolge|Ordnungsrelation |Sozialstatus|
|Intervall|+Abstände|Gleichheit von Differenzen|Einkommen|
|Metrisch|+absoluter Nullpunkt|Gleichheit von Verhältnissen|Längenmaß|

* Es ist möglich ein hohes Skalenniveau in ein niedrigeres zu transferieren

## Erhebungsmethoden
* Beobachtung: qualitativ vs quantitativ
* Befragung: mündlich vs. schriftlich
* Experimentelle designs: psycholgische tests, physiologische Messung
* Interviewform
  - nicht-standardisiertes Interview (narrativ)
  - offenes Interview 
  - halbstandardisiertes Interview (Leitfaden)
  - standardisiertes interview
  
## Schriftliche Befragung
* Wenn möglich validierte Instrumente

## Gütekriterien
* Objektivität: Anwenderunabhängig
* Reliabilität: Wiederholbarkeit
* Validität: Gültig

## Deskriptive Statistik
* Kurze Beschreibung der grundlegenden Datenmerkmalen
* Datenaufbereitung
* Berechnung von statistischen Kennzahlen
* Grundlagen jeder umfangreicheren quantitativen Datenanalyse

## Statistische Datenanalyse
* Univariat
  - Maße der zentralen Tendenz (Lagemaße)
  - Dispersionsmaße (Streungsmaße)
  - Proportionen, Häufigkeiten
* Bivariat
  - Analyse von Unterschieden
  - Zusammenahngsanalyse
* Multivariat
  - Struktur entdeckende Verfahren
  - Strukturprüfende Verfahren
  
## Lage und Streuungsmaße
* Modalwert (höchster Wert)
* Median 
* Mittelwert

* Varianz ist die Summe der quadrierten Abweichungen vom Mittelwert
* Standardabweichung ist die Wurzel aus der Varianz (wieder in der Standardeinheit)


## Methodenberatung
[Methodenberatung der Universität Zürich](https://www.methodenberatung.uzh.ch/de.html)

## Normalverteilung
* Glockenförmig
* Unimodal
* Symetrisch

## Konfidenzintervall und p-Wert
* p-Wert gibt die Wahrscheinlichekti an eine Falschaussage zu treffen
* Konfidenzintervall gibt Informationen über die Größe eine Effektes
* Alternative Baysean statistics

## Wahl der Analysemethode
* Siehe Methodenberatung Universtität Zürich

## t-Test
* Der t-Test vergleicht Mittelwerte
* Bei 2 unabhängigen Gruppen - Zweisitchprobentest
* Bei 2 abhängigen Gruppen - Gepaarte Stichproben
* Bei 1 Gruppe
* Klassische Frage: Wie wahrscheinlich ist die empirisch gefundene oder eine größere Mittelwertdifferenz unter allen möglichen rein theoretisch denkbaren Differenzen?
* Voraussetzungen des t-Tests
  - Die abhängige Variable ist intervallskaliert
  - Das untersuchte Merkmal ist in den Grundgesamtheiten der beiden Gruppen normalverteilt
  - Homogenität der Varianzen (->Leven Test)
  - Die einzelnen Messwerte sind voneinander unabhängig
  
## Korrelation
* Man nimmt den Korrelationskoeffizient zur Abschätzung der Stärke eines Zusammenhangs (nimmt Werte zwischen -1 und +1 an)
* Korrelationskoeffizent r
* Interpretation nach Cohen, aber abhängig vom Untersuchungsgegenstand

## Chi-Quadrat-Test
* Der Chi-Quadrat-Test wird zur Überprüfung von Häufigkeitsverteilungen eingesetzt also bei Variablen mit nomalem Skalenniveau
* Typische Frage: Tragen Männer oder Frauen häufiger Brillen

## Lineare Regression
* Kann angewendet werden, wenn die abhängige Variable metrisch ist. 

## Logistische Regression
* Kann angewendet werden, wenn die abhängige Variable dichotom ist
* Sinnvoll für viele medizinische Fragestellungen: Hat die Person ein Übergewicht oder nicht