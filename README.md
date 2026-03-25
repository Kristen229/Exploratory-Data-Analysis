# 🛒 Analyse Exploratoire de Données — Instacart Courses en Ligne

## 📋 Aperçu

Ce projet réalise une **Analyse Exploratoire de Données (EDA)** sur le jeu de données [Instacart Market Basket Analysis](https://www.kaggle.com/datasets/psparks/instacart-market-basket-analysis) afin de découvrir les habitudes d'achat des clients et fournir des recommandations business exploitables.

L'analyse explore **plus de 3,4 millions de commandes** provenant de **plus de 200 000 utilisateurs** pour répondre à des questions clés sur les comportements d'achat, la popularité des produits et les tendances des produits biologiques.

## 🔍 Questions Clés Explorées

| # | Question | Résultat Principal |
|---|----------|-------------------|
| 1 | **Quand les utilisateurs font-ils leurs courses ?** | Pic de commandes le dimanche et lundi, entre 10h et 15h |
| 2 | **Combien d'articles par commande ?** | Moyenne de 10 articles ; la plupart des commandes sont de taille moyenne (5–14 articles) |
| 3 | **Produits les plus vendus ?** | Les fruits et légumes frais dominent le top 20 |
| 4 | **Fréquence de réachat ?** | Moyenne de 15 jours entre les commandes |
| 5 | **Premier article ajouté au panier ?** | Les bananes et produits bio sont systématiquement choisis en premier |
| 6 | **Part des produits biologiques ?** | ~30% des commandes contiennent au moins un produit bio |
| 7 | **Produits par département ?** | Soins Personnels possède le plus grand nombre de produits distincts |

## 📊 Exemples de Visualisations

Le notebook inclut plus de 10 visualisations couvrant :
- Distribution des commandes par jour et heure (diagrammes en barres, graphiques linéaires)
- Catégorisation de la taille des commandes (histogrammes, diagrammes circulaires)
- Analyse des produits phares (diagrammes en barres horizontales)
- Distribution de la fréquence de réachat
- Répartition bio vs. non-bio
- Cartes de chaleur croisées (heure × jour)

## 🗂️ Jeu de Données

L'analyse utilise 5 fichiers CSV du dataset Instacart :

| Fichier | Description | Taille |
|---------|-------------|--------|
| `orders.csv` | Métadonnées des commandes (utilisateur, jour, heure, fréquence) | ~109 Mo |
| `order_products.csv` | Produits de chaque commande | ~578 Mo |
| `products.csv` | Catalogue produits avec noms | ~2 Mo |
| `aisles.csv` | Table de référence des rayons | ~3 Ko |
| `departments.csv` | Table de référence des départements | ~270 o |

> **Note** : Les fichiers CSV ne sont pas inclus dans ce dépôt en raison de leur taille. Téléchargez-les depuis [Kaggle](https://www.kaggle.com/datasets/psparks/instacart-market-basket-analysis) et placez-les dans un dossier `DATASET/`.

## 🚀 Démarrage Rapide

### Prérequis

- Python 3.8+
- Jupyter Notebook ou JupyterLab

### Installation

```bash
# Cloner le dépôt
git clone https://github.com/YOUR_USERNAME/Exploratory-Data-Analysis.git
cd Exploratory-Data-Analysis

# Installer les dépendances
pip install -r requirements.txt

# Télécharger le dataset depuis Kaggle et placer les fichiers dans DATASET/

# Lancer le notebook
jupyter notebook analysis_project.ipynb
```

## 🛠️ Stack Technique

- **Python 3** — Langage principal
- **Pandas** — Manipulation et agrégation de données
- **Matplotlib** — Bibliothèque de visualisation de base
- **Seaborn** — Visualisations statistiques
- **Plotly** — Graphiques interactifs

## 📁 Structure du Projet

```
Exploratory-Data-Analysis/
├── DATASET/                    # Fichiers de données CSV (non suivis par git)
│   ├── aisles.csv
│   ├── departments.csv
│   ├── order_products.csv
│   ├── orders.csv
│   └── products.csv
├── analysis_project.ipynb      # Notebook d'analyse principal
├── requirements.txt            # Dépendances Python
├── .gitignore
└── README.md
```

## 📝 Insights Clés & Recommandations

1. **Stratégie de Timing** : Les commandes atteignent leur pic le dimanche et lundi matin. Les promotions devraient cibler le samedi soir pour capter le cycle de planification hebdomadaire.
2. **Optimisation du Panier** : La plupart des commandes contiennent 5–14 articles. Des offres groupées dans cette fourchette pourraient augmenter la valeur moyenne des commandes.
3. **Croissance du Bio** : Les produits biologiques représentent une petite part du catalogue mais apparaissent fréquemment dans les paniers — élargir l'offre bio pourrait générer des revenus supplémentaires.
4. **Cycles de Réachat** : Le cycle moyen de réachat de 15 jours suggère que des rappels/promotions bimensuels seraient efficaces.


## 👤 Auteur

**Kristen OKE** — Analyste de Données

- GitHub : https://github.com/Kristen229
- LinkedIn : https://www.linkedin.com/in/kristen-oke-a3337b377/

