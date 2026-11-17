# L9 — Diagnostic de la qualité des données

**Projet :** Analyse des départs des salariés — BI RH  
**Méthodologie :** CRISP-DM — Data Understanding  
**Outil :** Google Colab (Python)

## 1. Objectif

Ce diagnostic vise à évaluer la qualité du dataset IBM HR Analytics Employee Attrition & Performance avant son exploitation dans Power BI.

Les contrôles portent sur les valeurs manquantes, les doublons, les valeurs atypiques et les incohérences métier.

## 2. Vérification des valeurs manquantes

La méthode `df.isnull().sum()` a été utilisée pour rechercher les valeurs manquantes dans les différentes colonnes.

**Résultat : aucune valeur manquante détectée.**

## 3. Vérification des doublons

Deux contrôles ont été réalisés :

- Recherche des lignes entièrement dupliquées avec `df.duplicated()`.
- Recherche des identifiants dupliqués avec `df["EmployeeNumber"].duplicated()`.

| Contrôle | Résultat |
|---|---:|
| Lignes dupliquées | 0 |
| Identifiants dupliqués | 0 |
| Identifiants manquants | 0 |

Les 1 470 salariés possèdent des identifiants uniques.

## 4. Détection des valeurs atypiques

La méthode de l'écart interquartile (IQR) a été appliquée aux variables `Age`, `YearsAtCompany` et `MonthlyIncome`.

Les valeurs situées en dehors des bornes suivantes sont considérées comme atypiques :

- Borne inférieure = Q1 − 1,5 × IQR
- Borne supérieure = Q3 + 1,5 × IQR

| Variable | Valeurs atypiques |
|---|---:|
| Age | 0 |
| YearsAtCompany | 104 |
| MonthlyIncome | 114 |

Les valeurs atypiques ne seront pas supprimées automatiquement, car elles peuvent correspondre à des situations professionnelles réelles.

## 5. Vérification des incohérences métier

### 5.1 Âge des salariés

- Âge minimum : 18 ans.
- Âge maximum : 60 ans.
- Âges inférieurs à 18 ans ou supérieurs à 65 ans : 0.

Aucune incohérence détectée selon la règle appliquée.

### 5.2 Ancienneté

- Anciennetés négatives : 0.
- Anciennetés supérieures à l'âge du salarié : 0.

Aucune incohérence détectée selon les contrôles effectués.

### 5.3 Satisfaction professionnelle

La variable `JobSatisfaction` contient uniquement les niveaux 1, 2, 3 et 4.

Nombre de valeurs invalides : 0.

### 5.4 Variables catégorielles

Les variables `Attrition` et `OverTime` contiennent uniquement les catégories `Yes` et `No`.

Nombre de valeurs invalides : 0 pour chacune.

## 6. Synthèse du diagnostic

| Dimension de qualité | Résultat |
|---|---|
| Valeurs manquantes | Aucune détectée |
| Doublons | Aucun détecté |
| Unicité des identifiants | Respectée |
| Valeurs atypiques | 104 pour l'ancienneté et 114 pour le revenu |
| Cohérence des âges | Conforme aux règles testées |
| Cohérence de l'ancienneté | Conforme aux règles testées |
| Validité des catégories | Conforme aux règles testées |

## 7. Décisions de préparation des données

À la suite du diagnostic :

- Aucune imputation de valeurs manquantes n'est nécessaire.
- Aucune suppression de doublons n'est nécessaire.
- Les valeurs atypiques seront conservées à ce stade.
- Des vérifications complémentaires pourront être réalisées pendant la préparation des données dans Power BI.

## 8. Conclusion

Le dataset présente une bonne qualité structurelle selon les contrôles réalisés.

Aucune valeur manquante ni aucun doublon n'a été détecté. Les contrôles métier n'ont pas révélé d'incohérences selon les règles testées.

Les valeurs atypiques observées pour l'ancienneté et le revenu mensuel nécessitent une attention particulière, mais ne constituent pas nécessairement des erreurs.

Le dataset peut donc être utilisé pour poursuivre les analyses RH, sous réserve des vérifications complémentaires nécessaires.

**Source :** notebook `Data_Understanding.ipynb`, sections L9 — Diagnostic de la qualité des données et Vérification des incohérences métier.
