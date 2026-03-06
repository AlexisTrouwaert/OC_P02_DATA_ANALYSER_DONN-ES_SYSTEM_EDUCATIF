# 🎓 Academy Market Analysis : Stratégie d'Expansion Internationale

Ce projet vise à accompagner l'entreprise **Academy**, une start-up EdTech, dans l'identification des marchés prioritaires pour son déploiement à l'international. L'analyse repose sur le traitement massif des données de la Banque Mondiale (EdStats).

---

## Problématique Business
L'enjeu est de déterminer quels pays présentent le meilleur équilibre entre :
1. **Un bassin d'utilisateurs massif** (Volume d'élèves au secondaire).
2. **Une faisabilité technique optimale** (Infrastructure Internet).
3. **Un potentiel de conversion élevé** (Investissement des familles dans l'éducation).

## Stack Technique
* **Langage** : Python 3.11+ 
* **Gestionnaire de projet** : `uv` (reproductibilité garantie via `pyproject.toml`)
* **Librairies Data** : 
    * `pandas` & `numpy` (Analyse et manipulation)
    * `matplotlib` & `seaborn` (Visualisation et Heatmap)
    * `scikit-learn` (Normalisation Min-Max)

## Méthodologie
Le projet suit un pipeline rigoureux de Data Analysis :
1. **Nettoyage (Cleaning)** : Filtrage de 880 000 lignes pour isoler la fenêtre temporelle 2010-2015.
2. **Sélection** : Réduction de 4 000 à 10 indicateurs clés basés sur la pertinence métier et l'analyse de corrélation (Heatmap).
3. **Scoring Hybride** : 
    * **Modèle A** : Score pondéré favorisant l'infrastructure Internet (x3) et le volume scolaire (x2.5).
    * **Modèle B** : Calcul de récurrence dans les tops mondiaux.
4. **Triangulation** : Sélection finale du Top 5 basée sur la convergence des deux modèles.

## Résultats & Recommandations
Le Top 5 des pays cibles identifiés est : **Estonie, Lituanie, Croatie, Chili, Espagne**.

| Marché | Rôle Stratégique |
| :--- | :--- |
| **Estonie / Lituanie** | **Phase de Test** : Marchés "Early Adopters" avec infrastructure parfaite. |
| **Espagne** | **Phase de Scale** : Marché à fort volume pour la rentabilité. |
| **Chili** | **Diversification** : Porte d'entrée prioritaire pour l'Amérique Latine. |

## Installation & Utilisation
Ce projet utilise `uv` pour une gestion efficace de l'environnement virtuel.

1. **Installer uv** (si pas déjà fait).
2. **Synchroniser l'environnement** :
   ```bash
   uv sync