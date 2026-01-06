## 📧 Deep Learning — Classification de spam (DNN avec Keras)

Ce dépôt contient deux notebooks complémentaires illustrant la mise en œuvre d’un réseau de neurones dense (DNN) pour un problème classique de classification binaire : détection de spam.

L’objectif n’est pas de “faire du deep learning pour faire du deep learning”, mais de montrer :

une implémentation claire et maîtrisée avec Keras,

l’impact des callbacks sur l’apprentissage,

une démarche progressive et pédagogique.

-> pip install numpy pandas scikit-learn tensorflow

### 📌 Notebook 1 — DNN de base (spam_1_DNN_Keras_base.ipynb)
🎯 Objectif

Mettre en place un réseau de neurones dense simple pour la classification de spam, sans mécanismes avancés de régularisation automatique.

🔧 Pipeline général

Chargement et préparation des données

Séparation train / test

Définition d’un Dense Neural Network avec Keras

Compilation du modèle (loss, optimizer, métrique)

Entraînement classique avec fit()

Évaluation des performances sur le jeu de test

🧠 Points clés

Architecture lisible et volontairement simple

Base de référence pour comparer les effets des callbacks

Apprentissage “brut”, sans contrôle fin de l’overfitting

👉 Ce notebook sert de baseline claire et compréhensible.

### 📌 Notebook 2 — DNN avec callbacks (spam_2_DNN_Keras_callback.ipynb)
🎯 Objectif

Améliorer et contrôler l’apprentissage du modèle précédent à l’aide de callbacks Keras.

🧪 Callbacks utilisés

EarlyStopping
→ arrêt automatique de l’entraînement lorsque la performance stagne

(éventuellement) sauvegarde du meilleur modèle

Suivi plus fin de la généralisation

🔁 Différences avec le notebook 1

Entraînement plus stable

Réduction du risque d’overfitting

Temps de calcul mieux maîtrisé

Modèle final sélectionné sur des critères objectifs

👉 Ce notebook montre une approche plus professionnelle du deep learning, proche des pratiques en production ou en projet réel.

### 📊 Comparaison implicite des approches

| Aspect                    | DNN de base | DNN avec callbacks          |
| ------------------------- | ----------- | --------------------------- |
| Simplicité                | ✅           | ⚠️ légèrement plus complexe |
| Contrôle de l’overfitting | ❌           | ✅                           |
| Robustesse                | Moyenne     | Élevée                      |
| Bonnes pratiques DL       | Partielle   | Complète                    |
