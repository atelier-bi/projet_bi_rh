# L4 — Catalogue des indicateurs KPI

## Objectif
Définir les principaux indicateurs RH permettant de mesurer et d'analyser l'attrition des salariés à partir du jeu de données IBM HR Analytics.

## Catalogue des KPI

| KPI | Définition / Calcul | Variables utilisées |
|---|---|---|
| Effectif total | Nombre total de salariés | EmployeeNumber |
| Nombre de départs | Nombre de salariés dont Attrition = Yes | Attrition |
| Taux d'attrition | (Nombre de départs / Effectif total) × 100 | Attrition |
| Taux d'attrition par département | (Départs du département / Effectif du département) × 100 | Attrition, Department |
| Taux d'attrition par poste | (Départs du poste / Effectif du poste) × 100 | Attrition, JobRole |
| Taux d'attrition par genre | (Départs du genre / Effectif du genre) × 100 | Attrition, Gender |
| Âge moyen des salariés | Moyenne des âges | Age |
| Revenu mensuel moyen | Moyenne des revenus mensuels | MonthlyIncome |
| Ancienneté moyenne | Moyenne des années dans l'entreprise | YearsAtCompany |
| Taux d'attrition avec heures supplémentaires | (Départs parmi les salariés en heures supplémentaires / Effectif de ce groupe) × 100 | Attrition, OverTime |
| Taux d'attrition par satisfaction | (Départs par niveau de satisfaction / Effectif du niveau) × 100 | Attrition, JobSatisfaction |
| Taux d'attrition par équilibre vie professionnelle/personnelle | (Départs par niveau / Effectif du niveau) × 100 | Attrition, WorkLifeBalance |

## Utilisation dans Power BI
Les indicateurs seront présentés à l'aide de cartes KPI, de graphiques en barres et de filtres interactifs.

## Règles de calcul
- Le taux d'attrition est calculé sur le groupe analysé.
- Les valeurs Attrition = Yes indiquent les salariés ayant quitté l'entreprise dans le jeu de données.
- Les indicateurs décrivent le jeu de données disponible, sans représenter une évolution temporelle réelle.

## Limites
Le jeu de données ne contient pas de dates individuelles de départ permettant de calculer un taux de rotation annuel réel. Les comparaisons permettent d'identifier des associations et non des causalités.
