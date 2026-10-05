<!-- ELUCENIA technical documentation · gasto-energetico · fr · no clinical/professional/rights approval -->

# Dépense énergétique (Mifflin-St Jeor et Harris-Benedict)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/gasto-energetico)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Sexe

`sexo`

- `F` — Féminin
- `M` — Masculin

### Âge

`idade`

ans · intervalle: 18–100

### Poids

`peso`

kg · intervalle: 30–300

### Taille

`altura`

cm · intervalle: 120–230

### Niveau d’activité physique (PAL)

`pal`

- `1.53` — Sédentaire ou léger (PAL 1,53)
- `1.76` — Actif ou modérément actif (NAP 1,76)
- `2.25` — Intense (PAL 2,25)

## Édition de la méthode

Mifflin–St Jeor 1990 et Harris–Benedict révisée Roza–Shizgal 1984 ; PAL FAO/OMS/UNU 2004

## Formule documentée

Mifflin–St Jeor: 10 × poids (kg) + 6,25 × taille (cm) − 5 × âge + 5 (hommes) ou − 161 (femmes).

Harris–Benedict révisée (Roza et Shizgal, 1984): hommes 88,362 + 13,397 × poids + 4,799 × taille − 5,677 × âge; femmes 447,593 + 9,247 × poids + 3,098 × taille − 4,330 × âge.

Dépense totale = dépense au repos × PAL (FAO/OMS/UNU 2004 : sédentaire 1,40 à 1,69; actif 1,70 à 1,99; intense 2,00 à 2,40).

## Limites et population

L’équation de Mifflin a été développée chez des adultes sains de 19–78 ans, de poids normal ou obèses, avec le poids en kg, la taille en cm et l’âge en années. Elle n’équivaut pas à une calorimétrie individuelle et ne démontre pas son adéquation chez les enfants, pendant la grossesse ou en maladie critique. Les autres équations et facteurs d’activité doivent suivre leurs propres sources et populations.

## Références

- [Mifflin MD et al. A new predictive equation for resting energy expenditure in healthy individuals. Am J Clin Nutr, 1990.](https://doi.org/10.1093/ajcn/51.2.241)

- [Roza AM, Shizgal HM. The Harris Benedict equation reevaluated: resting energy requirements and the body cell mass. Am J Clin Nutr, 1984.](https://doi.org/10.1093/ajcn/40.1.168)

- [FAO/WHO/UNU. Human energy requirements: report of a Joint FAO/WHO/UNU Expert Consultation. Roma, 2004.](https://www.fao.org/4/y5686e/y5686e00.htm)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
