<!-- ELUCENIA technical documentation · gasto-energetico · es · no clinical/professional/rights approval -->

# Gasto energético (Mifflin-St Jeor y Harris-Benedict)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/gasto-energetico)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Sexo

`sexo`

- `F` — Femenino
- `M` — Masculino

### Edad

`idade`

años · intervalo: 18–100

### Peso

`peso`

kg · intervalo: 30–300

### Estatura

`altura`

cm · intervalo: 120–230

### Nivel de actividad física (PAL)

`pal`

- `1.53` — Sedentario o ligero (PAL 1,53)
- `1.76` — Activo o moderadamente activo (PAL 1,76)
- `2.25` — Vigoroso (PAL 2,25)

## Edición del método

Mifflin–St Jeor 1990 y Harris–Benedict revisada Roza–Shizgal 1984; PAL FAO/OMS/UNU 2004

## Fórmula documentada

Mifflin–St Jeor: 10 × peso (kg) + 6,25 × altura (cm) − 5 × edad + 5 (hombres) o − 161 (mujeres).

Harris–Benedict revisada (Roza y Shizgal, 1984): hombres 88,362 + 13,397 × peso + 4,799 × altura − 5,677 × edad; mujeres 447,593 + 9,247 × peso + 3,098 × altura − 4,330 × edad.

Gasto total = gasto en reposo × PAL (FAO/OMS/UNU 2004: sedentario 1,40 a 1,69; activo 1,70 a 1,99; vigoroso 2,00 a 2,40).

## Límites y población

La ecuación de Mifflin se derivó en adultos sanos de 19–78 años, con peso normal y obesidad, utilizando peso en kg, altura en cm y edad en años. No equivale a calorimetría individual ni demuestra adecuación en niños, embarazo o enfermedad crítica. Las otras ecuaciones y los factores de actividad deben seguir sus propias fuentes y poblaciones.

## Referencias

- [Mifflin MD et al. A new predictive equation for resting energy expenditure in healthy individuals. Am J Clin Nutr, 1990.](https://doi.org/10.1093/ajcn/51.2.241)

- [Roza AM, Shizgal HM. The Harris Benedict equation reevaluated: resting energy requirements and the body cell mass. Am J Clin Nutr, 1984.](https://doi.org/10.1093/ajcn/40.1.168)

- [FAO/WHO/UNU. Human energy requirements: report of a Joint FAO/WHO/UNU Expert Consultation. Roma, 2004.](https://www.fao.org/4/y5686e/y5686e00.htm)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
