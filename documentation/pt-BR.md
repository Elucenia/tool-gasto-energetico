<!-- ELUCENIA technical documentation · gasto-energetico · pt-BR · no clinical/professional/rights approval -->

# Gasto energético (Mifflin-St Jeor e Harris-Benedict)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/gasto-energetico)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Sexo

`sexo`

- `F` — Feminino
- `M` — Masculino

### Idade

`idade`

anos · intervalo: 18–100

### Peso

`peso`

kg · intervalo: 30–300

### Altura

`altura`

cm · intervalo: 120–230

### Nível de atividade física (PAL)

`pal`

- `1.53` — Sedentário ou leve (PAL 1,53)
- `1.76` — Ativo ou moderado (PAL 1,76)
- `2.25` — Vigoroso (PAL 2,25)

## Edição do método

Mifflin St Jeor 1990 e Harris Benedictrevisada Roza Shizgal 1984; PALFAOWHOUNU 2004

## Fórmula documentada

Mifflin-St Jeor: 10 × peso (kg) + 6,25 × altura (cm) − 5 × idade + 5 (homens) ou − 161 (mulheres).

Harris-Benedict revisada (Roza e Shizgal, 1984): homens 88,362 + 13,397 × peso + 4,799 × altura − 5,677 × idade; mulheres 447,593 + 9,247 × peso + 3,098 × altura − 4,330 × idade.

Gasto total = gasto de repouso × PAL (FAO/OMS/UNU 2004: sedentário 1,40 a 1,69; ativo 1,70 a 1,99; vigoroso 2,00 a 2,40).

## Limites e população

A equação de Mifflin foi derivada em adultos saudáveis de 19–78 anos, com peso normal e obesidade, utilizando peso em kg, altura em cm e idade em anos. Não equivale a calorimetria individual nem comprova adequação em crianças, gestação ou doença crítica. As outras equações e fatores de atividade devem seguir suas próprias fontes e populações.

## Referências

- [Mifflin MD et al. A new predictive equation for resting energy expenditure in healthy individuals. Am J Clin Nutr, 1990.](https://doi.org/10.1093/ajcn/51.2.241)

- [Roza AM, Shizgal HM. The Harris Benedict equation reevaluated: resting energy requirements and the body cell mass. Am J Clin Nutr, 1984.](https://doi.org/10.1093/ajcn/40.1.168)

- [FAO/WHO/UNU. Human energy requirements: report of a Joint FAO/WHO/UNU Expert Consultation. Roma, 2004.](https://www.fao.org/4/y5686e/y5686e00.htm)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Gasto total estimado: 3.045 kcal/dia (PAL 1,76)

| Detalhes do resultado | |
| --- | --- |
| Harris-Benedict revisada (repouso) | 1.797 kcal/dia |
| Harris-Benedict × PAL | 3.162 kcal/dia |
| Mifflin-St Jeor × PAL | 3.045 kcal/dia |

Equações derivadas em adultos saudáveis: em doentes críticos, obesos graves e idosos frágeis, prefira calorimetria indireta ou as metas por kg das diretrizes.


### 2

Gasto total estimado: 2.020 kcal/dia (PAL 1,53)

| Detalhes do resultado | |
| --- | --- |
| Harris-Benedict revisada (repouso) | 1.384 kcal/dia |
| Harris-Benedict × PAL | 2.117 kcal/dia |
| Mifflin-St Jeor × PAL | 2.020 kcal/dia |

Equações derivadas em adultos saudáveis: em doentes críticos, obesos graves e idosos frágeis, prefira calorimetria indireta ou as metas por kg das diretrizes.


### 3

Gasto total estimado: 3.864 kcal/dia (PAL 2,25)

| Detalhes do resultado | |
| --- | --- |
| Harris-Benedict revisada (repouso) | 1.847 kcal/dia |
| Harris-Benedict × PAL | 4.155 kcal/dia |
| Mifflin-St Jeor × PAL | 3.864 kcal/dia |

Equações derivadas em adultos saudáveis: em doentes críticos, obesos graves e idosos frágeis, prefira calorimetria indireta ou as metas por kg das diretrizes.

