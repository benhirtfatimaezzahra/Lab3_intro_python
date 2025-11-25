# calcul de réduction de prix

calcul de réduction de prix est un mini-projet Python qui calcule le prix final d'un produit en appliquant différentes réductions selon le profil du client : statut étudiant, fidélité, et prix initial.

Ce projet a pour objectif de pratiquer les bases du langage Python : saisie utilisateur, conversions de types, conditions multiples, logique booléenne et gestion des erreurs.

---

##  Fonctionnalités

- Saisie du prix du produit.
- Vérification du statut étudiant (o/n).
- Saisie des années de fidélité du client.
- Application de trois règles de réduction :
  - **10 %** pour les étudiants.
  - **15 %** pour les clients fidèles (fidélité **≥ 5 années**).
  - **5 €** si le prix initial dépasse **100 €**.
- Réductions **cumulatives**.
- Garde-fou : le prix final ne peut jamais devenir négatif.
- Affichage :
  - Réduction totale en euros.
  - Prix final formaté à deux décimales.

---

##  Architecture
```
calcul_de_réduction_de_prix.ipynb → Script principal contenant :
- Lecture et validation des entrées (try/except)
- Application des règles de réduction
- Accumulation progressive des remises
- Calcul du prix final
- Bloc anti-prix négatif
- Affichage final des résultats
```

---

## Installation

Cloner le projet :
```bash
git clone https://github.com/benhirtfatimaezzahra/Lab3_intro_python.git
```

Ouvrir le notebook avec Jupyter :
```bash
cd Lab3_intro_python
jupyter notebook calcul_de_réduction_de_prix.ipynb
```

Ou utilisez JupyterLab :
```bash
jupyter lab calcul_de_réduction_de_prix.ipynb
```

---

---

##  Démonstration

Une vidéo illustrant le fonctionnement du programme peut être ajoutée dans le dépôt :


https://github.com/user-attachments/assets/1359f9eb-a964-447f-a483-5f6eec081273

---

##  Notes

- `float()` et `int()` sont utilisés pour convertir les entrées utilisateur.
- `strip()` et `lower()` servent à nettoyer et normaliser les réponses (o/n).
- Les règles de réduction sont indépendantes, donc toutes appliquées si les conditions sont remplies.
- Le garde-fou final assure que le prix ne descend jamais en dessous de 0 €.

Ce script est idéal pour comprendre :
- les conditions (`if`, `>=`, `>`)
- les pourcentages
- la logique Python simple
- la validation utilisateur avec `try/except`

---

##  Auteur

**Nom :** Benhirt Fatima-Ezzahra  
**Cours :** Introduction à Python  
**Date :** Novembre 2025  
**Encadré par :** Pr. Mohamed LACHGAR
