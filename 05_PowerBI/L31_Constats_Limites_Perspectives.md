# L31 — Constats, limites et perspectives

**Projet :** Analyse des départs des salariés — BI RH  
**Sprint :** Sprint 1 — Compréhension des données  
**Méthodologie :** CRISP-DM et Scrum  
**Outil :** Power BI

## 1. Objectif

Ce document présente les principaux constats issus de l'exploration du jeu de données RH, les limites identifiées et les prochaines étapes du projet.

L'objectif est de préparer la phase de Data Preparation du Sprint 2.

## 2. Principaux constats

L'analyse exploratoire porte sur un jeu de données fictif de 1 470 salariés.

### 2.1. Taux global d'attrition

- Effectif total : 1 470 salariés.
- Nombre de départs : 237 salariés.
- Nombre de salariés restés : 1 233.
- Taux global d'attrition : 16,12 %.

Ces résultats montrent qu'environ 16 salariés sur 100 sont identifiés comme ayant quitté l'entreprise dans le jeu de données.

### 2.2. Attrition par département

Les taux d'attrition observés sont :

| Département | Taux d'attrition |
|---|---:|
| Sales | 20,63 % |
| Human Resources | 19,05 % |
| Research & Development | 13,84 % |

Le département Sales présente le taux d'attrition le plus élevé.

Cependant, il est important de prendre en compte les effectifs de chaque département pour interpréter correctement ces différences.

### 2.3. Attrition selon l'ancienneté

Les salariés ayant entre 0 et 2 ans d'ancienneté présentent un taux d'attrition de 29,82 %.

Ce résultat suggère que les premières années dans l'entreprise constituent une période à examiner en priorité.

### 2.4. Heures supplémentaires

Le taux d'attrition observé est de :

- 30,53 % chez les salariés effectuant des heures supplémentaires.
- 10,44 % chez les salariés n'effectuant pas d'heures supplémentaires.

Cette différence indique une association entre les heures supplémentaires et l'attrition, sans démontrer un lien de causalité.

## 3. Diagnostic de qualité des données

Les contrôles réalisés lors de la phase Data Understanding ont permis d'observer :

- Aucune valeur manquante détectée.
- Aucun doublon complet détecté.
- 104 valeurs atypiques signalées pour `YearsAtCompany`.
- 114 valeurs atypiques signalées pour `MonthlyIncome`.

Ces valeurs atypiques ne sont pas nécessairement des erreurs. Elles devront être examinées avant toute décision de traitement.

## 4. Limites de l'analyse

### 4.1. Données fictives

Le dataset IBM HR Analytics est fictif. Les résultats ne doivent donc pas être généralisés directement à une entreprise réelle.

### 4.2. Absence d'historique temporel

Le jeu de données ne contient pas de dates précises de départ.

Il n'est donc pas possible d'étudier l'évolution mensuelle ou annuelle de l'attrition.

### 4.3. Absence de causalité

Les relations observées entre l'attrition, l'ancienneté, les départements ou les heures supplémentaires sont descriptives.

Elles ne permettent pas de déterminer avec certitude les causes des départs.

### 4.4. Analyse exploratoire

Le travail réalisé au Sprint 1 vise principalement à comprendre les données et à identifier des tendances.

Il ne constitue pas encore une analyse prédictive ou un système décisionnel final.

## 5. Prochaines étapes — Sprint 2

Le Sprint 2 sera consacré à la phase Data Preparation de CRISP-DM.

Les principales actions envisagées sont :

1. Examiner les valeurs atypiques identifiées.
2. Vérifier et harmoniser les types de données.
3. Documenter les règles de nettoyage.
4. Préparer les données dans Power Query.
5. Vérifier la cohérence des données après transformation.
6. Préparer le modèle de données Power BI.
7. Définir les premières mesures DAX nécessaires aux KPI RH.
8. Mettre à jour les livrables GitHub et les tâches Jira.

## 6. Conclusion

Le Sprint 1 a permis de mieux comprendre les caractéristiques des salariés et d'identifier plusieurs profils présentant des taux d'attrition élevés.

Les résultats mettent notamment en évidence des différences selon les départements, l'ancienneté et les heures supplémentaires.

Ces observations constituent une première base pour orienter les analyses RH.

Le Sprint 2 permettra de préparer les données et de renforcer la fiabilité des analyses avant la construction du tableau de bord décisionnel final.
