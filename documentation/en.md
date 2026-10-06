<!-- ELUCENIA technical documentation · gasto-energetico · en · no clinical/professional/rights approval -->

# Energy expenditure (Mifflin–St Jeor and Harris–Benedict)

[conditions, sources and permissions](https://elucenia.org/en/tools/gasto-energetico)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Sex

`sexo`

- `F` — Female
- `M` — Male

### Age

`idade`

years · range: 18–100

### Weight

`peso`

kg · range: 30–300

### Height

`altura`

cm · range: 120–230

### Physical activity level (PAL)

`pal`

- `1.53` — Sedentary or light (PAL 1.53)
- `1.76` — Active or moderately active (PAL 1.76)
- `2.25` — Vigorous (PAL 2.25)

## Method edition

Mifflin–St Jeor 1990 and revised Harris–Benedict Roza–Shizgal 1984; PAL FAO/WHO/UNU 2004

## Documented formula

Mifflin–St Jeor: 10 × weight (kg) + 6.25 × height (cm) − 5 × age + 5 (men) or − 161 (women).

Revised Harris–Benedict (Roza and Shizgal, 1984): men 88.362 + 13.397 × weight + 4.799 × height − 5.677 × age; women 447.593 + 9.247 × weight + 3.098 × height − 4.330 × age.

Total expenditure = resting expenditure × PAL (FAO/WHO/UNU 2004: sedentary 1.40 to 1.69; active 1.70 to 1.99; vigorous 2.00 to 2.40).

## Limits and population

The Mifflin equation was derived in healthy adults aged 19–78 years, with normal weight and obesity, using weight in kg, height in cm and age in years. It is not equivalent to individual calorimetry and does not establish suitability in children, pregnancy or critical illness. Other equations and activity factors must follow their own sources and populations.

## References

- [Mifflin MD et al. A new predictive equation for resting energy expenditure in healthy individuals. Am J Clin Nutr, 1990.](https://doi.org/10.1093/ajcn/51.2.241)

- [Roza AM, Shizgal HM. The Harris Benedict equation reevaluated: resting energy requirements and the body cell mass. Am J Clin Nutr, 1984.](https://doi.org/10.1093/ajcn/40.1.168)

- [FAO/WHO/UNU. Human energy requirements: report of a Joint FAO/WHO/UNU Expert Consultation. Roma, 2004.](https://www.fao.org/4/y5686e/y5686e00.htm)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Estimated total expenditure: 3045 kcal/day (PAL 1.76)

| Result details | |
| --- | --- |
| Revised Harris-Benedict (resting) | 1797 kcal/day |
| Harris-Benedict × PAL | 3162 kcal/day |
| Mifflin-St Jeor × PAL | 3045 kcal/day |

Equations derived in healthy adults: in critically ill patients, severe obesity and frail older adults, prefer indirect calorimetry or the per-kg targets from the guidelines.


### 2

Estimated total expenditure: 2020 kcal/day (PAL 1.53)

| Result details | |
| --- | --- |
| Revised Harris-Benedict (resting) | 1384 kcal/day |
| Harris-Benedict × PAL | 2117 kcal/day |
| Mifflin-St Jeor × PAL | 2020 kcal/day |

Equations derived in healthy adults: in critically ill patients, severe obesity and frail older adults, prefer indirect calorimetry or the per-kg targets from the guidelines.


### 3

Estimated total expenditure: 3864 kcal/day (PAL 2.25)

| Result details | |
| --- | --- |
| Revised Harris-Benedict (resting) | 1847 kcal/day |
| Harris-Benedict × PAL | 4155 kcal/day |
| Mifflin-St Jeor × PAL | 3864 kcal/day |

Equations derived in healthy adults: in critically ill patients, severe obesity and frail older adults, prefer indirect calorimetry or the per-kg targets from the guidelines.

