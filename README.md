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

# 🎓 Academy Market Analysis: International Expansion Strategy

This project aims to support **Academy**, an EdTech start-up, in identifying priority markets for its international deployment. The analysis is based on the processing of the World Bank's **EdStats** database.

---

## 🚀 Business Problem
The challenge is to determine which countries present the best balance between:
1. **Massive user base** (Secondary education enrollment volume).
2. **Optimal technical feasibility** (Internet infrastructure).
3. **High conversion potential** (Families' investment in education and private institutions).

## 🛠️ Technical Stack
* **Language**: Python 3.11+
* **Project Manager**: `Poetry` (Ensuring reproducibility via `pyproject.toml`)
* **Data Libraries**: 
    * `pandas` & `numpy` (Analysis and manipulation)
    * `matplotlib` & `seaborn` (Visualization and Heatmap)
    * `scikit-learn` (Min-Max Normalization)

## 📊 Methodology
The project follows a rigorous Data Analysis pipeline:
1. **Cleaning**: Filtering 880,000 rows to isolate the 2010-2015 time window for data completeness.
2. **Selection**: Reducing 4,000 indicators to 10 key metrics based on business relevance and correlation analysis (Heatmap).
3. **Hybrid Scoring**: 
    * **Model A**: Weighted score favoring Internet infrastructure (x3) and school volume (x2.5).
    * **Model B**: Recurrence count in global Top 15 rankings.
4. **Triangulation**: Final Top 5 selection based on the convergence of both models.

## 🏆 Key Results & Recommendations
The final Top 5 priority markets identified are: **Estonia, Lithuania, Croatia, Chile, and Spain**.

| Market | Strategic Role |
| :--- | :--- |
| **Estonia / Lithuania** | **Test Phase**: "Early Adopters" with perfect digital infrastructure. |
| **Spain** | **Scale Phase**: Large demographic market to drive profitability. |
| **Chile** | **Diversification**: Natural gateway for the Latin American region. |

## 💻 Installation & Usage
This project uses `Poetry` for efficient virtual environment management.

1. **Install Poetry** (if not already installed).
2. **Synchronize the environment**:
   ```bash
   poetry install
