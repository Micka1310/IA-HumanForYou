# Livrable 2 – Notebook Jupyter
# IA for HumanForYou : Prédiction du Turnover

**Notebook associé** : `notebooks/L2-Partie1.ipynb`

## Sommaire

### PHASE 1 : Cadrage et étude des données

1. Introduction et contexte  
   1.1 Présentation de HumanForYou  
   1.2 Problème du turnover (15 % annuel)  
   1.3 Enjeux métier et impact du projet  

2. Problématique et objectifs  
   2.1 Problématique centrale  
   2.2 Objectifs techniques  
   2.3 Objectifs éthiques (AI Act 2024)  
   2.4 Vue d’ensemble de la démarche  

3. Audit éthique des variables  
   3.1 Rappel des catégories du Livrable 1  
   3.2 Analyse des corrélations sensibles / proxy  
   3.3 Décisions d’exclusion ou de surveillance  
   3.4 Impact attendu sur la modélisation 

4. Présentation des jeux de données  
   4.1 Description des 5 fichiers  
       4.1.1 general_data.csv  
       4.1.2 manager_survey_data.csv  
       4.1.3 employee_survey_data.csv  
       4.1.4 in_time.csv  
       4.1.5 out_time.csv  
   4.2 Variable cible : Attrition  
   4.3 Typologie des variables (sensibles, proxy, organisationnelles)  
 

5. Stratégie de segmentation et fusion des datasets  
   5.1 Séparation en deux familles  
   5.2 Fusion RH (fichiers au grain employé)  
   5.3 Agrégation des données horaires (in_time / out_time)  
   5.4 Construction du dataset final df_final   

---

### PHASE 2 : Préparation et modélisation

6. Préprocessing des données  
   6.1 Gestion des valeurs manquantes  
   6.2 Feature engineering  
   6.3 Encodage des variables catégorielles  
   6.4 Standardisation / normalisation  
   6.5 Split train / test (80/20 stratifié)  

7. Exploration des données (EDA)  
   7.1 Analyse univariée  
   7.2 Analyse bivariée  
   7.3 Corrélations et distributions  
   7.4 Observations métier préliminaires 

8. Modèle 1 : Régression Logistique  
   8.1 Rappel théorique  
   8.2 Entraînement et configuration  
   8.3 Évaluation (F1, AUC, matrice de confusion)  
   8.4 Interprétation des coefficients  
   8.5 Discussion (avantages / limites)  

9. Modèle 2 : Random Forest  
   9.1 Rappel théorique  
   9.2 Entraînement et configuration  
   9.3 Évaluation (F1, AUC, matrice de confusion)  
   9.4 Importance des variables et interprétation  
   9.5 Discussion (avantages / limites)  

---

### PHASE 3 : Évaluation, éthique et recommandations

10. Analyse comparative des modèles  
    10.1 Tableau comparatif des métriques  
    10.2 Analyse des erreurs  
    10.3 Choix du modèle retenu 

11. Optimisation du modèle et Pipeline de Livraison
    12.1 Mesures correctives  
    12.2 Test et benchmark
    12.3 Pipeline et mise en production
    12.4 Proposition d'interface / IHM Canva pour dept. RH

12. Évaluation éthique et équité  
    11.1 Analyse de l’équité par groupes  
    11.2 Vérification des 7 exigences de l’AI Act  
    11.3 Points de vigilance et limites éthiques  

13. Recommandations métier pour HumanForYou  
    12.1 Principaux facteurs de risque identifiés  
    12.2 Leviers RH concrets  
    12.3 Guide d’usage du modèle en pratique  

14. Limites et perspectives  
    13.1 Limites des données et des modèles  
    13.2 Pistes d’amélioration technique  
    13.3 Pistes d’amélioration organisationnelle  

15. Conclusion générale  
    14.1 Bilan technique  
    14.2 Bilan éthique  
    14.3 Apports pour HumanForYou

***