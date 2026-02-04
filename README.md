PROJET FINAL : ALGORITHME DE SCORE ÉDITORIAL (ANIME)
Auteur : Justin BANDIOLA
Date : Février 2026

------------------------------------------------------------------------
1. CONTEXTE ET OBJECTIF
------------------------------------------------------------------------
Ce projet vise à aider une plateforme de streaming à identifier les "Pépites" 
de son catalogue.
Le problème identifié : La note globale (moyenne) est trompeuse car elle masque 
l'irrégularité de certains animés.

Ma solution : Créer un "Score Éditorial" qui pénalise l'instabilité.
Hypothèse : Un animé avec une note de 9/10 mais très irrégulier est plus risqué 
qu'un animé à 8.8/10 très constant (comme "Steins;Gate").

------------------------------------------------------------------------
2. MÉTHODOLOGIE & LOGIQUE MÉTIER
------------------------------------------------------------------------
J'ai développé un algorithme de classification basé sur trois étapes :
1. Calcul du Risque : Différence entre la note du meilleur et du pire épisode.
2. Création du Score : Note Globale - (10% de l'écart type).
3. Segmentation : Classification automatique en 4 catégories :
   - 💎 PÉPITE (Note haute + Grande stabilité)
   - ✅ Valeur Sûre
   - ⚠️ Risqué (Trop d'écart de qualité)
   - ❌ Fond de catalogue

------------------------------------------------------------------------
3. INSTRUCTIONS D'INSTALLATION & LANCEMENT
------------------------------------------------------------------------
Pour exécuter l'analyse sur votre machine :

PRÉREQUIS :
- Avoir Python installé (via Anaconda ou Jupyter Desktop).
- Avoir le fichier "animes.csv" dans le même dossier.

INSTALLATION DES LIBRAIRIES :
Ouvrir un terminal ou une cellule Jupyter et lancer :
pip install pandas matplotlib seaborn wordcloud

LANCEMENT :
1. Ouvrir le fichier "Projet Anime Justin BANDIOLA.ipynb".
2. Cliquer sur "Run All" (Exécuter tout).
3. Le script générera les graphiques et le fichier "resultat_final_projet.csv".

------------------------------------------------------------------------
FICHIERS INCLUS :
1. Notebook Jupyter (Code complet + Analyses)
2. CSV Nettoyé (Résultats finaux)
3. README.txt (Ce document)
