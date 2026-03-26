# Chiffrement par Substitution – Projet Master

## Description
Ce projet met en œuvre un **chiffrement par substitution** inspiré des méthodes classiques de cryptographie. Il permet de :

- Chiffrer un texte en utilisant une clé secrète.
- Déchiffrer un texte à l’aide de la clé.
- Estimer le contenu d’un texte chiffré grâce à une **analyse fréquentielle**, illustrant la vulnérabilité du chiffrement par substitution face à la cryptanalyse statistique.

Le projet est réalisé dans le cadre du Master « Big Data, Analyse et Business Intelligence ».

---

## Fonctionnalités

1. **Chiffrement**
   - Transformation d’un texte clair en texte chiffré via une clé.
   - Gestion des lettres accentuées et préservation de la ponctuation.
   
2. **Déchiffrement**
   - Décryptage avec la clé secrète.
   - Restauration complète du texte original.

3. **Analyse fréquentielle**
   - Déchiffrement approximatif d’un texte sans clé, basé sur les fréquences typiques des lettres en français.
   - Illustration de la vulnérabilité du chiffrement par substitution face à la cryptanalyse.

---

## Structure du projet
