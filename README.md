# 📊 Analyse BI du Marché Immobilier Marocain — Power BI

## 📌 Description du Projet

Ce projet consiste à exploiter les données du Data Warehouse construites à partir des annonces immobilières de Avito.ma afin de réaliser une analyse décisionnelle avec Power BI.

Le projet utilise uniquement le schéma :

- `bi_schema` → dédié à la Business Intelligence (BI)

Le schéma :

- `ml_schema` → réservé au Machine Learning

n’est pas utilisé dans cette partie.

L’objectif principal est de créer des tableaux de bord interactifs permettant d’analyser le marché immobilier marocain.

---

# 🏗️ Architecture du Projet

## 📂 Schémas Utilisés

### ✅ BI Schema (`bi_schema`)

Schéma optimisé pour l’analyse décisionnelle.

### Structure utilisée :
- Modèle en étoile (Star Schema)
- Modèle Snowflake
- Modèle Galaxy (si nécessaire)

### Contient :
- Tables de dimensions
- Tables de faits

---

### ❌ ML Schema (`ml_schema`)

One Big Table (OBT) destiné au Machine Learning.

➡️ Non utilisé dans ce brief.

---

# 🛠️ Technologies Utilisées


- Power Query
- DAX (Data Analysis Expressions)
- Data Warehouse

---

# 🔌 Connexion au Data Warehouse

## Étapes

1. Ouvrir :contentReference[oaicite:4]{index=4} Desktop
2. Cliquer sur **Obtenir des données**
3. Choisir la base de données :
   - PostgreSQL
   - SQL Server
   - DuckDB
4. Importer uniquement les tables du :
   - `bi_schema`
5. Vérifier :
   - les clés primaires
   - les relations
   - les cardinalités

---

# 🧹 Préparation des Données avec Power Query

## 🎯 Objectifs

Utilisation de Power Query pour :

- Nettoyer les incohérences restantes
- Vérifier les types des colonnes
- Supprimer les doublons
- Filtrer les valeurs aberrantes
- Renommer les colonnes
- Créer des colonnes calculées
- Optimiser le modèle Power BI

---

# 📐 Colonnes Calculées

## 📌 Exemple : Prix par m²

```powerquery
Prix_m2 = [price] / [surface]
```

---

# 📈 Dashboards Réalisés

---

# 📊 Dashboard 1 — Vue Globale du Marché

## 📌 Contenu

- Nombre total d’annonces
- Prix moyen du marché
- Répartition des annonces par ville
- Evolution temporelle des annonces
- KPIs principaux

## 📊 Visualisations

- Cards
- Bar Chart
- Line Chart
- Pie Chart
- KPI Cards

---

# 📊 Dashboard 2 — Analyse des Prix

## 📌 Contenu

- Distribution des prix
- Prix moyen par m²
- Comparaison des segments immobiliers

## 📊 Visualisations

- Histogramme
- Bar Chart
- pie chart
- KPI

---

# 📊 Dashboard 3 — Analyse Géographique

## 📌 Contenu

- Répartition des annonces par ville
- Carte des prix immobiliers
- Zones les plus chères

## 📊 Visualisations
-kpi
- Map
- Treemap
- Bar Chart

---

# 📊 Dashboard 4 — Analyse Comparative du marché Immobillier

## 📌 Contenu
-la Somme de prix par surface
- Evolution des  moyenne prix par les villes
- Evolution du volume des annonces par ville
- Total Annonces par catégorie de prix
## 📊 Visualisations

- Line Chart
- Pie Chart
- KPI
- Nuage de points

---

# 🎛️ Filtres Interactifs

Les dashboards contiennent des filtres dynamiques :

- Ville
- Type de bien
- catégorie de prix
- Surface
-

✅ Tous les graphiques sont connectés et réactifs aux filtres sélectionnés.

---

# 📂 Structure du Projet

```bash
project/
│
│── immobilier_dashboard.pbix
│
├── screenshots/
│
├── README.md
```

---

# 📸 Captures d’Écran

## 🖥️ Dashboard Global

<img width="1419" height="796" alt="image" src="https://github.com/user-attachments/assets/78d333cd-72d4-4a8e-9cb5-7df303f026db" />


---

## 💰 Dashboard Prix

<img width="1398" height="794" alt="image" src="https://github.com/user-attachments/assets/74854a45-c01b-429a-86e1-40b0e1edae5e" />


---

## 🌍 Dashboard Géographique

<img width="1415" height="788" alt="image" src="https://github.com/user-attachments/assets/5cd78b5d-e094-4ddc-90b8-ab78732ca4ae" />


---

## 📈 Dashboard Tendances

<img width="1405" height="778" alt="image" src="https://github.com/user-attachments/assets/2a5a6b1d-6bdb-40b0-9e9d-e74c4d2ead8e" />


---

# 🚀 Résultats du Projet

Le projet permet :

- Une analyse complète du marché immobilier marocain
- Une visualisation interactive des données
- Une aide à la prise de décision
- Une détection des tendances immobilières

---

# 📚 Concepts Utilisés

- Business Intelligence
- Data Warehouse
- ETL
- Power Query
- DAX
- Data Visualization
- KPI
- Dashboarding

---

# 📌 Conclusion

Ce projet permet de transformer les données brutes des annonces immobilières en informations décisionnelles exploitables grâce à Power BI, Power Query et DAX.

Les dashboards interactifs facilitent l’analyse du marché immobilier marocain et l’identification des tendances importantes.

---

