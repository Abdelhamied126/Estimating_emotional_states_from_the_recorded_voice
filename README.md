

#  Reconnaissance des Émotions à partir de la Voix

## Description du TP

Ce projet vise à analyser et reconnaître les émotions humaines à partir de données vocales. Le travail a été réalisé dans le cadre de **[indiquez le contexte, par exemple, un stage ou un projet académique]**. Deux modèles d’intelligence artificielle ont été développés et comparés : un modèle **LSTM** et un modèle basé sur des transformateurs, **Wave2Vec2**, pour déterminer lequel est le plus performant dans la classification des émotions.

Ce projet a permis de mettre en lumière les forces et limites de ces modèles selon les données et les cas d’usage.  

---

## Objectifs du Projet

1. Mettre en œuvre un modèle **LSTM** basé sur des coefficients MFCC pour capturer les dépendances temporelles dans les données vocales.
2. Adapter et évaluer le modèle **Wave2Vec2** pour le traitement direct des formes d’onde audio.
3. Comparer les deux approches selon des métriques comme la précision, le rappel et le F1-score.
4. Analyser les résultats pour recommander les meilleures pratiques en reconnaissance d'émotions vocales.

---

## Méthodes et Technologies Utilisées

### Modèle LSTM :
- **Prétraitement des données** :
  - Extraction des **MFCC** à l’aide de la bibliothèque `librosa`.
  - Normalisation du taux d’échantillonnage à 22 050 Hz.
- **Architecture du modèle** :
  - Couches LSTM empilées pour capturer les dépendances temporelles.
  - Régularisation via **Dropout**, **Batch Normalization**, et **Early Stopping**.
- **Entraînement** :
  - Optimisation avec **Adam** et surveillance des métriques d'évaluation.

### Modèle Wave2Vec2 :
- **Prétraitement des données** :
  - Conversion des fichiers audio au format brut avec un échantillonnage à 16 kHz.
- **Fine-tuning** :
  - Adaptation d’un modèle pré-entraîné sur une tâche de classification d'émotions.
  - Augmentation des données pour réduire l’overfitting.

---

## Résultats

- **LSTM** : 
  - Précision sur les données de test : **83%**.
  - Bonne généralisation malgré quelques confusions entre émotions proches (ex. : peur et joie).
- **Wave2Vec2** :
  - Performances initiales impressionnantes mais surapprentissage dû à la complexité du modèle et à la taille limitée des données.

---



Lien vers le compte rendu complet sur Google Drive : [Cliquez ici pour accéder au compte rendu](#) *(https://drive.google.com/file/d/1YajqQmNABGG8M2vmmouwHvGNTxbM8bXR/view?usp=drive_link)*.

---



## Auteur 

- **Auteur** : Omar Yousif Abdehamied.  
- **Collaboration** : Marmara University et ENSEA, Cergy.

