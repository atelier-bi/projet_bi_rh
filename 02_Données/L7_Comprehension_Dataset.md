# L7 — Présentation et compréhension du dataset

## 1. Objectif

Cette étape consiste à comprendre la structure et le contenu du jeu de données IBM HR Analytics Employee Attrition & Performance avant de commencer les analyses dans Power BI.

## 2. Présentation générale

Le dataset contient des informations relatives aux salariés d'une entreprise et à leur situation professionnelle.

| Caractéristique | Description |
|---|---|
| Nom | IBM HR Analytics Employee Attrition & Performance |
| Format | CSV |
| Nombre de lignes | 1 470 |
| Nombre de colonnes | 35 |
| Domaine | Ressources humaines |
| Variable cible | Attrition |
| Unité d'observation | Un salarié |

Chaque ligne représente un salarié et chaque colonne correspond à une caractéristique.

## 3. Principales variables

| Variable | Signification |
|---|---|
| EmployeeNumber | Identifiant du salarié |
| Age | Âge du salarié |
| Gender | Genre |
| Department | Département |
| JobRole | Poste occupé |
| MonthlyIncome | Revenu mensuel |
| YearsAtCompany | Ancienneté dans l'entreprise |
| JobSatisfaction | Niveau de satisfaction professionnelle |
| WorkLifeBalance | Équilibre entre vie professionnelle et personnelle |
| OverTime | Réalisation d'heures supplémentaires |
| Attrition | Départ ou maintien du salarié |

## 4. Variable cible : Attrition

La variable `Attrition` permet de distinguer deux catégories :

- **Yes :** salarié ayant quitté l'entreprise.
- **No :** salarié n'ayant pas quitté l'entreprise.

Elle constitue la variable principale de notre projet.

## 5. Types de données

Le dataset contient plusieurs types de variables :

- **Numériques :** `Age`, `MonthlyIncome`, `YearsAtCompany`.
- **Catégorielles :** `Gender`, `Department`, `JobRole`.
- **Binaires :** `Attrition`, `OverTime`.
- **Ordinales :** `JobSatisfaction`, `WorkLifeBalance`.

Cette distinction est importante pour choisir les traitements et les visualisations appropriés.

## 6. Analyses envisagées

À partir de ces variables, nous pourrons étudier :

- Le taux global d'attrition.
- L'attrition selon le département et le poste.
- Les différences d'attrition selon l'âge et le genre.
- La relation entre l'ancienneté et les départs.
- L'association entre les heures supplémentaires et l'attrition.
- Le lien entre la satisfaction professionnelle et les départs.

## 7. Outils et méthode

L'exploration initiale des données est réalisée dans Google Colab à l'aide de Python.

Les analyses et les visualisations seront ensuite développées dans Power BI.

Cette étape correspond à la phase **Data Understanding** de la méthodologie CRISP-DM.

## 8. Limites

Le jeu de données ne contient pas de dates individuelles de départ permettant de réaliser une analyse temporelle réelle.

Les relations observées entre les variables ne permettent pas, à elles seules, d'établir des liens de causalité.

## 9. Conclusion

La compréhension du dataset permet d'identifier les variables pertinentes pour notre problématique RH et de préparer les étapes suivantes : exploration statistique, diagnostic de qualité et création des indicateurs Power BI.
