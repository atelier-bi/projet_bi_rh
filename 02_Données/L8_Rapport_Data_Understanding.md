# L8 — Rapport Data Understanding

**Projet :** Analyse des départs des salariés — BI RH  
**Méthodologie :** CRISP-DM  
**Outil d'exploration :** Google Colab (Python)

## 1. Objectif

Ce rapport présente les résultats de l'analyse exploratoire du jeu de données IBM HR Analytics Employee Attrition & Performance.

L'objectif est de comprendre les caractéristiques des salariés, de mesurer l'attrition et d'identifier les groupes présentant les proportions de départs les plus élevées.

## 2. Présentation du dataset

Le dataset comprend **1 470 salariés et 35 variables**.

Chaque ligne correspond à un salarié. La variable `Attrition` indique si le salarié a quitté l'entreprise (`Yes`) ou non (`No`).

La variable `EmployeeNumber` permet d'identifier les salariés de manière unique.

## 3. Statistiques générales

| Indicateur | Résultat |
|---|---:|
| Effectif total | 1 470 |
| Nombre de départs | 237 |
| Salariés restants | 1 233 |
| Proportion globale de départs | 16,12 % |
| Âge moyen | 36,92 ans |
| Ancienneté moyenne | 7,01 ans |
| Revenu mensuel moyen | 6 502,93 |
| Revenu mensuel médian | 4 919 |

**Interprétation :** environ 16 salariés sur 100 sont identifiés comme ayant quitté l'entreprise dans le dataset. Le revenu mensuel moyen est supérieur à la médiane, ce qui indique une distribution influencée par les revenus élevés.

## 4. Analyse de l'attrition par département

| Département | Proportion de départs |
|---|---:|
| Sales | 20,63 % |
| Human Resources | 19,05 % |
| Research & Development | 13,84 % |

Le département Research & Development possède le plus grand effectif, avec 961 salariés et 133 départs.

Cependant, **Sales présente la proportion de départs la plus élevée (20,63 %)**. Ce département constitue donc un groupe prioritaire à examiner.

## 5. Analyse selon l'ancienneté

| Ancienneté | Effectif | Départs | Proportion |
|---|---:|---:|---:|
| 0–2 ans | 342 | 102 | 29,82 % |
| 3–5 ans | 434 | 60 | 13,82 % |
| 6–10 ans | 448 | 55 | 12,28 % |
| 11–20 ans | 180 | 12 | 6,67 % |
| 21 ans et plus | 66 | 8 | 12,12 % |

**Interprétation :** les salariés ayant entre 0 et 2 ans d'ancienneté présentent la proportion de départs la plus élevée, soit 29,82 %.

À l'inverse, le groupe ayant entre 11 et 20 ans d'ancienneté présente la proportion la plus faible, avec 6,67 %.

Ces résultats suggèrent que les salariés récemment recrutés méritent une attention particulière dans les analyses RH.

## 6. Analyse selon la satisfaction professionnelle

| Niveau de satisfaction | Effectif | Départs | Proportion |
|---|---:|---:|---:|
| 1 | 289 | 66 | 22,84 % |
| 2 | 280 | 46 | 16,43 % |
| 3 | 442 | 73 | 16,52 % |
| 4 | 459 | 52 | 11,33 % |

Les salariés ayant le niveau de satisfaction le plus faible (niveau 1) présentent une proportion de départs de **22,84 %**, contre **11,33 %** pour le niveau 4.

Ces résultats montrent une association entre la satisfaction professionnelle et l'attrition.

## 7. Analyse selon les heures supplémentaires

| Heures supplémentaires | Effectif | Départs | Proportion |
|---|---:|---:|---:|
| Non | 1 054 | 110 | 10,44 % |
| Oui | 416 | 127 | 30,53 % |

Les salariés effectuant des heures supplémentaires présentent une proportion de départs de **30,53 %**, contre **10,44 %** pour ceux qui n'en effectuent pas.

Les heures supplémentaires apparaissent ainsi comme une variable importante à approfondir dans le tableau de bord Power BI.

## 8. Principaux constats

L'analyse exploratoire met en évidence quatre observations principales :

1. Le département Sales présente la proportion de départs la plus élevée : 20,63 %.
2. Les salariés ayant 0 à 2 ans d'ancienneté présentent une proportion de départs de 29,82 %.
3. Les salariés ayant une faible satisfaction professionnelle présentent davantage de départs.
4. Les salariés effectuant des heures supplémentaires présentent une proportion de départs de 30,53 %.

Ces observations permettent de définir les axes prioritaires des prochaines analyses RH.

## 9. Limites de l'analyse

Le dataset ne précise pas la période d'observation et ne contient pas de dates individuelles de départ.

Les proportions calculées décrivent donc les départs présents dans le dataset, et non un taux de rotation annuel.

De plus, les associations observées ne permettent pas de conclure à des relations de cause à effet.

## 10. Conclusion

La phase Data Understanding a permis de mieux comprendre le dataset et d'identifier plusieurs variables pertinentes pour l'analyse de l'attrition.

Les résultats orienteront la conception du tableau de bord Power BI, notamment les analyses par département, ancienneté, satisfaction professionnelle et heures supplémentaires.

**Source des résultats :** notebook `Data_Understanding.ipynb`, analyses réalisées dans Google Colab.
