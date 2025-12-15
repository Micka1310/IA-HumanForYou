# Livrable 2 – Notebook Jupyter
# IA for HumanForYou : Prédiction du Turnover

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
   6.1 Rappel des catégories du Livrable 1  
   6.2 Analyse des corrélations sensibles / proxy  
   6.3 Décisions d’exclusion ou de surveillance  
   6.4 Impact attendu sur la modélisation 

4. Présentation des jeux de données  
   3.1 Description des 5 fichiers  
       3.1.1 general_data.csv  
       3.1.2 manager_survey_data.csv  
       3.1.3 employee_survey_data.csv  
       3.1.4 in_time.csv  
       3.1.5 out_time.csv  
   3.2 Variable cible : Attrition  
   3.3 Typologie des variables (sensibles, proxy, organisationnelles)  
 

5. Stratégie de segmentation et fusion des datasets  
   4.1 Séparation en deux familles  
   4.2 Fusion RH (fichiers au grain employé)  
   4.3 Agrégation des données horaires (in_time / out_time)  
   4.4 Construction du dataset final df_final   

---

### PHASE 2 : Préparation et modélisation

7. Préprocessing des données  
   7.1 Gestion des valeurs manquantes  
   7.2 Feature engineering  
   7.3 Encodage des variables catégorielles  
   7.4 Standardisation / normalisation  
   7.5 Split train / test (80/20 stratifié)  

8. Exploration des données (EDA)  
   5.1 Analyse univariée  
   5.2 Analyse bivariée  
   5.3 Corrélations et distributions  
   5.4 Observations métier préliminaires 

9. Modèle 1 : Régression Logistique  
   8.1 Rappel théorique  
   8.2 Entraînement et configuration  
   8.3 Évaluation (F1, AUC, matrice de confusion)  
   8.4 Interprétation des coefficients  
   8.5 Discussion (avantages / limites)  

10. Modèle 2 : Random Forest  
   9.1 Rappel théorique  
   9.2 Entraînement et configuration  
   9.3 Évaluation (F1, AUC, matrice de confusion)  
   9.4 Importance des variables et interprétation  
   9.5 Discussion (avantages / limites)  

---

### PHASE 3 : Évaluation, éthique et recommandations

11. Analyse comparative des modèles  
    10.1 Tableau comparatif des métriques  
    10.2 Analyse des erreurs  
    10.3 Choix du modèle retenu  

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