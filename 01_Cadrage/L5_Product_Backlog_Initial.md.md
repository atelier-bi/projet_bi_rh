# L5 — Product Backlog initial

**Projet :** Analyse des départs des salariés — BI RH  
**Méthodologie :** Scrum et CRISP-DM  
**Outil de suivi :** Jira (RHBI)

## 1. Objectif du Product Backlog

Le Product Backlog regroupe les besoins fonctionnels et analytiques du projet BI RH.

Il permet de prioriser les fonctionnalités nécessaires pour comprendre les départs des salariés et fournir aux responsables RH des informations utiles à la prise de décision.

## 2. User Stories initiales

| ID | User Story | Priorité | Estimation |
|---|---|---|---|
| US-01 | Définir les questions décisionnelles et les KPI RH | Haute | 3 SP |
| US-02 | Documenter le fichier RH et ses variables | Haute | 5 SP |
| US-03 | Vérifier la qualité du fichier RH | Haute | 5 SP |
| US-04 | Explorer les effectifs et les départs dans Power BI | Haute | 5 SP |

**Total : 18 Story Points**

Ces quatre User Stories correspondent aux tickets RHBI-1 à RHBI-4 du Sprint 1.

## 3. Description et critères d'acceptation

### US-01 — Définir les questions décisionnelles et les KPI RH

**En tant que** responsable RH,  
**je veux** disposer de questions décisionnelles et d'indicateurs RH pertinents,  
**afin de** mieux comprendre les départs des salariés.

**Critères d'acceptation :**
- Les principales questions décisionnelles sont documentées.
- Les KPI prioritaires sont identifiés.
- Chaque KPI possède une définition et une formule de calcul.
- Les indicateurs sont reliés aux besoins métier.

### US-02 — Documenter le fichier RH et ses variables

**En tant que** Data Analyst,  
**je veux** comprendre la structure et les variables du fichier RH,  
**afin de** préparer des analyses fiables.

**Critères d'acceptation :**
- La source du dataset est identifiée.
- Le nombre de lignes et de colonnes est documenté.
- Les types de données sont décrits.
- Un dictionnaire des données est disponible.

### US-03 — Vérifier la qualité du fichier RH

**En tant que** Data Analyst,  
**je veux** contrôler la qualité des données RH,  
**afin de** détecter les anomalies susceptibles d'influencer les analyses.

**Critères d'acceptation :**
- Les valeurs manquantes sont recherchées.
- Les doublons sont vérifiés.
- Les valeurs aberrantes sont analysées.
- Les résultats des contrôles sont documentés.

### US-04 — Explorer les effectifs et les départs dans Power BI

**En tant que** responsable RH,  
**je veux** visualiser les effectifs et les départs des salariés,  
**afin de** repérer les principales tendances d'attrition.

**Critères d'acceptation :**
- Le dataset RH est importé dans Power BI.
- Le nombre total de salariés est affiché.
- Le nombre de départs et le taux d'attrition sont calculés.
- Des graphiques présentent les départs selon des dimensions RH pertinentes.
- Le fichier Power BI est enregistré au format `.pbix`.

## 4. Priorisation

Les quatre User Stories sont considérées comme prioritaires pour le Sprint 1.

Les trois premières permettent de comprendre les besoins métier, de documenter les données et de vérifier leur qualité.

La quatrième permet de réaliser une première exploration visuelle dans Power BI.

## 5. Suivi dans Jira

Les User Stories sont suivies dans le projet Jira **RHBI**.

Leur avancement est contrôlé à l'aide du Sprint Backlog, du tableau Scrum et du Burndown Chart.

Les critères d'acceptation présentés ici constituent la base de vérification des livrables. Ils doivent être confirmés par le Product Owner et repris dans Jira.

## 6. Conclusion

Ce Product Backlog initial constitue une base de travail pour organiser le projet BI RH.

Il pourra être enrichi au cours des prochains sprints en fonction des résultats des analyses, des retours des parties prenantes et des nouveaux besoins identifiés.
