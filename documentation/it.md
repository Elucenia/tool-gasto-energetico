<!-- ELUCENIA technical documentation · gasto-energetico · it · no clinical/professional/rights approval -->

# Dispendio energetico (Mifflin-St Jeor e Harris-Benedict)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/gasto-energetico)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Sesso

`sexo`

- `F` — Femminile
- `M` — Maschile

### Età

`idade`

anni · intervallo: 18–100

### Peso

`peso`

kg · intervallo: 30–300

### Altezza

`altura`

cm · intervallo: 120–230

### Livello di attività fisica (PAL)

`pal`

- `1.53` — Sedentario o leggero (PAL 1,53)
- `1.76` — Attivo o moderatamente attivo (PAL 1,76)
- `2.25` — Intenso (PAL 2,25)

## Edizione del metodo

Mifflin–St Jeor 1990 e Harris–Benedict rivista Roza–Shizgal 1984; PAL FAO/OMS/UNU 2004

## Formula documentata

Mifflin–St Jeor: 10 × peso (kg) + 6,25 × altezza (cm) − 5 × età + 5 (uomini) o − 161 (donne).

Harris–Benedict rivista (Roza e Shizgal, 1984): uomini 88,362 + 13,397 × peso + 4,799 × altezza − 5,677 × età; donne 447,593 + 9,247 × peso + 3,098 × altezza − 4,330 × età.

Dispendio totale = dispendio a riposo × PAL (FAO/OMS/UNU 2004: sedentario 1,40 a 1,69; attivo 1,70 a 1,99; intenso 2,00 a 2,40).

## Limiti e popolazione

L’equazione di Mifflin è stata derivata in adulti sani di 19–78 anni, con peso normale e obesità, utilizzando peso in kg, altezza in cm ed età in anni. Non equivale alla calorimetria individuale e non dimostra l’adeguatezza in bambini, gravidanza o malattia critica. Le altre equazioni e i fattori di attività devono seguire le proprie fonti e popolazioni.

## Riferimenti

- [Mifflin MD et al. A new predictive equation for resting energy expenditure in healthy individuals. Am J Clin Nutr, 1990.](https://doi.org/10.1093/ajcn/51.2.241)

- [Roza AM, Shizgal HM. The Harris Benedict equation reevaluated: resting energy requirements and the body cell mass. Am J Clin Nutr, 1984.](https://doi.org/10.1093/ajcn/40.1.168)

- [FAO/WHO/UNU. Human energy requirements: report of a Joint FAO/WHO/UNU Expert Consultation. Roma, 2004.](https://www.fao.org/4/y5686e/y5686e00.htm)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Dispendio totale stimato: 3045 kcal/die (PAL 1,76)

| Dettagli del risultato | |
| --- | --- |
| Harris-Benedict rivista (riposo) | 1797 kcal/die |
| Harris-Benedict × PAL | 3162 kcal/die |
| Mifflin-St Jeor × PAL | 3045 kcal/die |

Equazioni derivate in adulti sani: nei pazienti critici, nell’obesità grave e negli anziani fragili, preferire la calorimetria indiretta o gli obiettivi per kg delle linee guida.


### 2

Dispendio totale stimato: 2020 kcal/die (PAL 1,53)

| Dettagli del risultato | |
| --- | --- |
| Harris-Benedict rivista (riposo) | 1384 kcal/die |
| Harris-Benedict × PAL | 2117 kcal/die |
| Mifflin-St Jeor × PAL | 2020 kcal/die |

Equazioni derivate in adulti sani: nei pazienti critici, nell’obesità grave e negli anziani fragili, preferire la calorimetria indiretta o gli obiettivi per kg delle linee guida.


### 3

Dispendio totale stimato: 3864 kcal/die (PAL 2,25)

| Dettagli del risultato | |
| --- | --- |
| Harris-Benedict rivista (riposo) | 1847 kcal/die |
| Harris-Benedict × PAL | 4155 kcal/die |
| Mifflin-St Jeor × PAL | 3864 kcal/die |

Equazioni derivate in adulti sani: nei pazienti critici, nell’obesità grave e negli anziani fragili, preferire la calorimetria indiretta o gli obiettivi per kg delle linee guida.

