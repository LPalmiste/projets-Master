
Chiffrement par Substitution – Projet Master
Description

Ce projet met en œuvre un chiffrement par substitution inspiré des méthodes classiques de cryptographie. Il permet de :

Chiffrer un texte en utilisant une clé secrète.
Déchiffrer un texte à l’aide de la clé.
Estimer le contenu d’un texte chiffré grâce à une analyse fréquentielle, illustrant la vulnérabilité du chiffrement par substitution face à la cryptanalyse statistique.

Le projet est réalisé dans le cadre du Master « Big Data, Analyse et Business Intelligence ».

Fonctionnalités
Chiffrement
Transformation d’un texte clair en texte chiffré via une clé.
Gestion des lettres accentuées et préservation de la ponctuation.
Déchiffrement
Décryptage avec la clé secrète.
Restauration complète du texte original.
Analyse fréquentielle
Déchiffrement approximatif d’un texte sans clé, basé sur les fréquences typiques des lettres en français.
Illustrations de la vulnérabilité du chiffrement par substitution face à la cryptanalyse.
Structure du projet
SubstitutionCipher/
 ├── main.py         # Script principal pour chiffrement et déchiffrement
 ├── README.md       # Présentation du projet
 └── examples/       # Exemples de texte chiffré et déchiffré (optionnel)
Installation
Cloner le dépôt :
git clone https://github.com/LPalmiste/projets-Master.git
cd projets-Master/SubstitutionCipher
Installer les dépendances Python (si nécessaire) :
pip install -r requirements.txt

Note : Le script n’utilise que des bibliothèques Python standard (unicodedata, collections).

Utilisation
Chiffrement et déchiffrement avec clé
from main import chiffrement, dechiffrement, alphabet_chiffrant, table_substitution

cle = "palmistelorie"
texte_clair = "Bonjour tout le monde"
AC = alphabet_chiffrant(cle)
table = table_substitution(AC)

texte_chiffre = chiffrement(texte_clair, table)
texte_dechiffre = dechiffrement(texte_chiffre, table)

print("Texte chiffré :", texte_chiffre)
print("Texte déchiffré :", texte_dechiffre)
Analyse fréquentielle
from main import dechiffrement_frequentiel

texte_estime, mapping_estime = dechiffrement_frequentiel(texte_chiffre)
print("Correspondances estimées :", mapping_estime)
print("Texte déchiffré approximatif :", texte_estime)
Exemple

Texte clair :
Bonjour tout le monde

Texte chiffré :
Uifotpsq xplv qspofe (exemple simplifié)

Texte déchiffré :
Bonjour tout le monde

Auteur

[Ton Nom]
Étudiant Master Big Data – Université Paris 13
