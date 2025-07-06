# Projet Deep Learning - Classification MNIST avec PyTorch

Ce projet implémente un modèle de classification d’images basé sur le dataset **MNIST**, en combinant **apprentissage supervisé** et **apprentissage semi-supervisé**, avec l’aide de la technique de **Virtual Adversarial Training (VAT)**. Le modèle est construit et entraîné avec **PyTorch**.

---

## 📌 Objectifs

- Entraîner un modèle robuste avec **peu de données étiquetées** (100 images, soit 10 par classe).
- Exploiter les données non-étiquetées via **VAT**, une méthode d’**apprentissage semi-supervisé**.
- Obtenir une bonne généralisation avec peu de supervision explicite.

---

## 🔍 Contenu du projet

Le projet comprend :

- Un **notebook Jupyter** (`Projet_deep_learning.ipynb`) avec tout le pipeline d'entraînement et d'évaluation.
- Un fichier **`best_model.pth`** contenant les poids du meilleur modèle sauvegardé.
- Ce fichier **README.md**.

---

## 🧪 Méthodologie

### 🔹 Données

- Dataset utilisé : [MNIST](http://yann.lecun.com/exdb/mnist/) (chiffres manuscrits, 28×28 pixels).
- **100 échantillons étiquetés** (10 par classe) extraits du jeu d’entraînement.
- Le reste des images est utilisé comme données **non étiquetées**.
- Jeu de test standard pour l’évaluation finale.

### 🔹 Apprentissage semi-supervisé avec VAT

Le modèle utilise la méthode **Virtual Adversarial Training (VAT)** pour apprendre à partir des données non-étiquetées.  
VAT consiste à perturber l'entrée dans une direction qui maximise la divergence entre la prédiction originale et la prédiction perturbée, tout en maintenant la cohérence du modèle.

Cela permet au modèle :
- de mieux **généraliser**,
- de **renforcer sa robustesse**,
- et d’**exploiter efficacement les données non-étiquetées**.

---

## ⚙️ Technologies utilisées

- [PyTorch](https://pytorch.org/)
- Torch
- NumPy
- matplotlib
- scikit-learn

## Auteurs

- **Aymane Mimoun**
- **Mohtadi Hammami**
- **Alexandre Combeau**

Master Data Science - Université Paris-Saclay 2025
