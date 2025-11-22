# Vrai-Devoir-2

## Question 3 : Problème 3 [30 points] — Prévision de prix basée sur l’apprentissage automatique

Dans cette question, vous explorerez si une approche d’apprentissage automatique peut surpasser le modèle simple BPA × P/B. En particulier, vous considérerez les régressions Ridge, LASSO et Elastic Net, dans le but d’améliorer la performance de prévision en utilisant des ensembles de caractéristiques plus riches.

### a. Création d’un ensemble de prédicteurs additionnels [5 points]
- Créez des prédicteurs au-delà du BPA et du P/B glissant.
- Exemples : termes au carré, décalages temporels, moyennes mobiles, variables indicatrices de secteur, mesures de volatilité, ou toute autre variable pertinente disponible.
- Expliquez et justifiez vos choix.

### b. Estimation des modèles Ridge, LASSO et Elastic Net [10 points]
- Utilisez votre ensemble de données construit pour estimer ces régressions.
- Sélectionnez les paramètres de pénalité optimaux via validation croisée.
- Rapportez l’EQMP hors échantillon pour chaque modèle.

### c. Comparaison avec le modèle de base via le test de Diebold-Mariano [5 points]
- Testez si le meilleur modèle de la partie (b) surpasse le modèle BPA × P/B.
- Interprétez la statistique de test et la valeur p.

### d. Discussion sur l’information ignorée et les raisons économétriques [5 points]
- Sur la base des résultats, les analystes ignorent-ils de l’information pertinente en se fiant au BPA × P/B ?
- Proposez au moins une raison économétrique (biais de variable omise, multicolinéarité, régression fallacieuse) pour laquelle le modèle simple peut sembler bien fonctionner, même s’il n’est pas le véritable PGD.

### e. Réflexion sur le compromis entre interprétabilité et performance
- Réfléchissez brièvement au compromis entre l’interprétabilité des modèles et leur performance prédictive.
