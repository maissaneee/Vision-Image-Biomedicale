# Traitement d’image industrielle et biomédicale – Vision par ordinateur

Projet réalisé dans le cadre du module “Vision informatique” (M1 Sciences Cognitives – IDMC, 2025).

## Objectifs généraux

1. Contrôle dimensionnel d’objets industriels (clés à molette) sur chaîne de production
2. Segmentation automatique de cellules basophiles sur images microscopiques bruitées

---

## Partie 1 – Contrôle industriel (clés)

### Objectif
Développer une chaîne de traitement permettant de :
- Extraire la clé du fond d’image malgré des défauts de capture
- Réaliser une calibration via image étalon (pièce de 45 mm)
- Délimiter une ROI pour extraire la zone utile
- Mesurer automatiquement la largeur de serrage des clés

### Méthodes utilisées
- Histogramme + profil d’intensité
- Segmentation par seuillage manuel et automatique (Otsu)
- Traitements morphologiques
- Détection de contours
- Calibration en mm/pixel

---

## Partie 2 – Analyse d’images biomédicales

### Objectif
Segmenter automatiquement les cellules basophiles sur des images bruitées pour :
- Aider au diagnostic
- Réduire le travail humain en laboratoire

### Méthodes explorées
- Filtrage (flou, seuillage adaptatif)
- Morphologie mathématique
- Suppression de bruit (OpenCV)
- Détection de formes et comptage

## Résultats
- Méthodes robustes aux variations d’éclairage sur les clés
- Segmentation partielle des basophiles avec détection des zones pertinentes

## Technologies
- Python, OpenCV, NumPy, Matplotlib
- Google Colab
