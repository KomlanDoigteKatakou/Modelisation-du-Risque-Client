# Modélisation du risque de crédit

## 🎯 Objectif
Construire un modèle de scoring pour estimer la probabilité de défaut (PD) des clients d’une banque, afin d’améliorer le processus de décision d’octroi de crédit.

## 🧠 Contexte
La banque souhaite anticiper le risque de non-remboursement de ses emprunteurs à partir de leurs caractéristiques socio-économiques et financières.  
L’enjeu est de passer d’un système de règles fixes à un modèle statistique robuste et interprétable.

## 🧮 Approche méthodologique
1. **Exploration des données**
   - Nettoyage, encodage, gestion des valeurs manquantes.  
   - Analyse de corrélations et détection des variables pertinentes (IV, WoE).  

2. **Modélisation**
   - Régression logistique (modèle de référence).  
   - Random Forest, XGBoost et CatBoost pour comparaison.  
   - Calibration des probabilités (Platt scaling, isotonic regression).  

3. **Évaluation**
   - AUC, Gini, Brier Score, ROC, KS.  
   - Validation croisée et analyse des erreurs.  
   - Interprétation des variables via SHAP values.  

4. **Scorecard**
   - Transformation des coefficients logistiques en score client.  
   - Seuil de décision optimisé selon le coût du risque.  

## 🧰 Technologies utilisées
- **Python** : Pandas, Scikit-learn, CatBoost, Matplotlib, SHAP  
- **Statistiques** : régression logistique, validation de modèle, calibration  

## 📊 Résultats visés
- AUC = 0.87 sur le jeu de test.  
- Scorecard interprétable et conforme aux standards Bâle II. 
