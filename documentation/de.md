<!-- ELUCENIA technical documentation · gasto-energetico · de · no clinical/professional/rights approval -->

# Energieverbrauch (Mifflin-St Jeor und Harris-Benedict)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/gasto-energetico)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Geschlecht

`sexo`

- `F` — Weiblich
- `M` — Männlich

### Alter

`idade`

Jahre · Bereich: 18–100

### Gewicht

`peso`

kg · Bereich: 30–300

### Körpergröße

`altura`

cm · Bereich: 120–230

### Körperliches Aktivitätsniveau (PAL)

`pal`

- `1.53` — Sitzend oder leicht (PAL 1,53)
- `1.76` — Aktiv oder mäßig aktiv (PAL 1,76)
- `2.25` — Intensiv (PAL 2,25)

## Fassung der Methode

Mifflin–St Jeor 1990 und revidierter Harris–Benedict Roza–Shizgal 1984; PAL FAO/WHO/UNU 2004

## Dokumentierte Formel

Mifflin–St Jeor: 10 × Gewicht (kg) + 6,25 × Größe (cm) − 5 × Alter + 5 (Männer) oder − 161 (Frauen).

Revidierter Harris–Benedict (Roza und Shizgal, 1984): Männer 88,362 + 13,397 × Gewicht + 4,799 × Größe − 5,677 × Alter; Frauen 447,593 + 9,247 × Gewicht + 3,098 × Größe − 4,330 × Alter.

Gesamtbedarf = Ruhebedarf × PAL (FAO/WHO/UNU 2004: sitzend 1,40 bis 1,69; aktiv 1,70 bis 1,99; sehr aktiv 2,00 bis 2,40).

## Grenzen und Population

Die Mifflin-Gleichung wurde bei gesunden normalgewichtigen und adipösen Erwachsenen von 19–78 Jahren mit Gewicht in kg, Größe in cm und Alter in Jahren entwickelt. Sie entspricht keiner individuellen Kalorimetrie und belegt keine Eignung bei Kindern, Schwangerschaft oder kritischer Krankheit. Andere Gleichungen und Aktivitätsfaktoren müssen ihren eigenen Quellen und Populationen folgen.

## Referenzen

- [Mifflin MD et al. A new predictive equation for resting energy expenditure in healthy individuals. Am J Clin Nutr, 1990.](https://doi.org/10.1093/ajcn/51.2.241)

- [Roza AM, Shizgal HM. The Harris Benedict equation reevaluated: resting energy requirements and the body cell mass. Am J Clin Nutr, 1984.](https://doi.org/10.1093/ajcn/40.1.168)

- [FAO/WHO/UNU. Human energy requirements: report of a Joint FAO/WHO/UNU Expert Consultation. Roma, 2004.](https://www.fao.org/4/y5686e/y5686e00.htm)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Geschätzter Gesamtenergieverbrauch: 3045 kcal/Tag (PAL 1,76)

| Ergebnisdetails | |
| --- | --- |
| Überarbeitete Harris-Benedict (Ruheumsatz) | 1797 kcal/Tag |
| Harris-Benedict × PAL | 3162 kcal/Tag |
| Mifflin-St Jeor × PAL | 3045 kcal/Tag |

Bei gesunden Erwachsenen abgeleitete Gleichungen: Bei kritisch Kranken, schwer adipösen und gebrechlichen älteren Erwachsenen indirekte Kalorimetrie oder die kg-Zielwerte der Leitlinien bevorzugen.


### 2

Geschätzter Gesamtenergieverbrauch: 2020 kcal/Tag (PAL 1,53)

| Ergebnisdetails | |
| --- | --- |
| Überarbeitete Harris-Benedict (Ruheumsatz) | 1384 kcal/Tag |
| Harris-Benedict × PAL | 2117 kcal/Tag |
| Mifflin-St Jeor × PAL | 2020 kcal/Tag |

Bei gesunden Erwachsenen abgeleitete Gleichungen: Bei kritisch Kranken, schwer adipösen und gebrechlichen älteren Erwachsenen indirekte Kalorimetrie oder die kg-Zielwerte der Leitlinien bevorzugen.


### 3

Geschätzter Gesamtenergieverbrauch: 3864 kcal/Tag (PAL 2,25)

| Ergebnisdetails | |
| --- | --- |
| Überarbeitete Harris-Benedict (Ruheumsatz) | 1847 kcal/Tag |
| Harris-Benedict × PAL | 4155 kcal/Tag |
| Mifflin-St Jeor × PAL | 3864 kcal/Tag |

Bei gesunden Erwachsenen abgeleitete Gleichungen: Bei kritisch Kranken, schwer adipösen und gebrechlichen älteren Erwachsenen indirekte Kalorimetrie oder die kg-Zielwerte der Leitlinien bevorzugen.

