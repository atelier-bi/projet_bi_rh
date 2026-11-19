# L16 — Product Backlog

**Projet :** Analyse des départs des salariés — BI RH  
**Formation :** Master 2 Business Analytics  
**Module :** Atelier Business Intelligence  
**Méthodologies :** Scrum et CRISP-DM  
**Outil :** Jira — Projet RHBI

## 1. Objectif

Le Product Backlog regroupe les besoins du projet BI RH sous forme de User Stories.

Il permet d'organiser et de prioriser les fonctionnalités nécessaires pour analyser les départs des salariés et aider la direction RH à prendre des décisions adaptées.

## 2. Product Backlog initial

| ID Jira | User Story | Priorité | Story Points |
|---|---|---|---:|
| RHBI-1 | US-01 — Définir les questions décisionnelles et les KPI RH | Haute | 3 |
| RHBI-2 | US-02 — Documenter le fichier RH et ses variables | Haute | 5 |
| RHBI-3 | US-03 — Vérifier la qualité du fichier RH | Haute | 5 |
| RHBI-4 | US-04 — Explorer les effectifs et les départs dans Power BI | Haute | 5 |
| **Total** | | | **18** |

## 3. Description des User Stories

### US-01 — Définir les questions décisionnelles et les KPI RH

**En tant que** responsable RH, je veux disposer d'indicateurs RH pertinents afin d'identifier les départements et les profils présentant des taux de départ élevés.

**Critères d'acceptation :**
- Les principales questions décisionnelles sont définies.
- Les KPI RH prioritaires sont identifiés.
- Chaque KPI possède une définition et une formule.
- Les indicateurs sont reliés aux objectifs métier.

### US-02 — Documenter le fichier RH et ses variables

**En tant que** Data Analyst, je veux comprendre la structure du fichier RH afin de préparer une analyse fiable.

**Critères d'acceptation :**
- La source du dataset est identifiée.
- Les 1 470 observations et les 35 variables sont documentées.
- Les types de données sont décrits.
- Un dictionnaire des données est disponible.

### US-03 — Vérifier la qualité du fichier RH

**En tant que** Data Analyst, je veux vérifier la qualité des données afin d'identifier les anomalies pouvant influencer les résultats.

**Critères d'acceptation :**
- Les valeurs manquantes sont contrôlées.
- Les doublons sont recherchés.
- Les valeurs atypiques sont identifiées.
- Un diagnostic de qualité est documenté.

### US-04 — Explorer les effectifs et les départs dans Power BI

**En tant que** responsable RH, je veux visualiser les effectifs et les départs afin d'identifier les principaux profils concernés par l'attrition.

**Critères d'acceptation :**
- Le dataset RH est importé dans Power BI.
- L'effectif total est affiché.
- Le nombre de départs et le taux d'attrition sont calculés.
- Des visualisations permettent de comparer les départs selon les départements et l'ancienneté.
- Un fichier Power BI au format `.pbix` est disponible.

## 4. Priorisation

Les quatre User Stories ont été sélectionnées pour le Sprint 1.

Les trois premières concernent le cadrage métier et la compréhension des données. La quatrième permet de réaliser une première exploration décisionnelle dans Power BI.

Cette organisation correspond aux premières phases de la méthodologie CRISP-DM.

## 5. Suivi

Les User Stories sont enregistrées dans le projet Jira RHBI.

Leur avancement est suivi à travers le Sprint Backlog, le tableau Scrum et le Burndown Chart.

Le Product Backlog pourra être enrichi lors des prochains sprints selon les besoins du projet.

## 6. Conclusion

Le Product Backlog définit les principales fonctionnalités du Sprint 1 et permet à l'équipe de travailler sur des objectifs communs.

Il constitue une base pour organiser les développements futurs et améliorer progressivement l'analyse des départs des salariés.
