# Problème 1 — Construction des données et analyse sommaire

## Objectif général
Reproduire les intrants empiriques utilisés dans l’article *Expected EPS × Trailing P/E Pricing Without Discounting* : collecte de données WRDS, construction des variables et analyse descriptive.

---

## **1.a — Sélection de l’échantillon et collecte des données**
Sélectionner aléatoirement **50 entreprises du S&P 500** et récupérer :
- Les **prix** (quotidiens ou mensuels selon l’article original)
- Le **bénéfice par action (BPA / EPS)**
- Le **ratio prix-bénéfice (P/B ou P/E) glissant**

Contraintes :
- Utiliser **WRDS** comme source principale
- Respecter la **fréquence** et **l’intervalle temporel** utilisés dans l’article
- Code adaptable à une taille d’échantillon différente

---

## **1.b — Construction des variables**
À partir des données de la partie (a) :
- Calculer les **rendements** pour chaque titre
- Estimer le **BPA attendu** (selon la définition de l’article : moyenne glissante, analyst forecasts, etc.)
- Calculer le **P/B glissant**
- Documenter clairement le code
- Spécifier les **hypothèses** ou approximations effectuées

---

## **1.c — Analyse descriptive**
Fournir pour chaque titre :
- Statistiques descriptives du **prix**, **rendement**, **BPA**, **P/B glissant**, et **BPA attendu × P/B**
- Graphiques de **séries temporelles** pour chaque variable
- Discussion des patterns :
  - Persistance
  - Valeurs aberrantes
  - Ralentissements / ruptures structurelles
  - Périodes de volatilité élevée

---

# Problème 2 — Prévision de prix de base utilisant BPA × P/B

## Objectif général
Tester l’affirmation centrale de l’article : **les prix sont principalement déterminés par le produit BPA attendu × P/B glissant**, sans actualisation traditionnelle.

---

## **2.a — Régression transversale groupée**
Modèle principal :
- Variable dépendante : **prix observé**
- Variable explicative : **BPA attendu × P/B glissant**

Rapporter :
- Coefficient estimé
- **R²**
- Statistiques des résidus
- Comparaison avec les résultats originaux de l’article

---

## **2.b — Modèles naïfs alternatifs**
Estimer deux modèles :
1. **Prix ~ P/B glissant**
2. **Prix ~ BPA seul**

Pour chaque modèle :
- Rapporter le **R²**
- Comparer les résultats au modèle de base
- Discuter du pouvoir explicatif conjoint du BPA attendu et du P/B glissant

---

## **2.c — Prévisions à une période d’avance**
Pour chacun des trois modèles (base + deux naïfs) :
- Construire les **prévisions 1-step ahead**
- Calculer l’**EQMP (RMSE)** hors-échantillon
- Identifier le modèle avec la meilleure performance
- Justifier cette conclusion par comparaison des EQMP

---

## **2.d — Graphique prix réels vs prévus**
Pour une entreprise représentative :
- Graphique comparant **prix observés** vs **prix prévus**
- Inclure des **intervalles de confiance à 95%** pour les prévisions
- Discussion :
  - Le modèle suit-il bien les prix ?
  - Présence d’erreurs persistantes ?
  - Modèle trop confiant (bandes trop étroites) ou pas assez confiant ?

---

