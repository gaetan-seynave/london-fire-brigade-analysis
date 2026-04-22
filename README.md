## London Fire Brigade — Analyse des temps de réponse

Projet réalisé dans le cadre du **Liora Data Analyst Bootcamp (Les Mines PSL, février 2026)**.

L'objectif était d'analyser les données publiques de la London Fire Brigade (LFB)
pour évaluer ses performances opérationnelles sur la période 2021–2025.

---

## Contexte

Ce projet s'inscrit dans ma reconversion en data analyse.
J'ai une expérience business de 15 ans (marketing, gestion de projet) et
une pratique de l'analyse de données développée en contexte professionnel réel.

La formation m'a permis de franchir une étape supplémentaire : structurer cette pratique
côté technique avec du preprocessing en Python, de la donnée brute au tableau de bord.

---

## Ce que j'ai analysé

La LFB publie ses données d'intervention en open data depuis 2009.
J'ai travaillé sur ~600 000 incidents et ~930 000 mobilisations sur 2021–2025.

Quelques questions explorées :
- Quels types d'incidents mobilisent le plus la brigade ?
- Les objectifs légaux de temps d'intervention sont-ils respectés ?
- Quels boroughs concentrent le plus de retards ?
- Le service est-il sous pression budgétaire ?

---

## Contenu du repo

 notebooks/
├── 01_preprocessing.ipynb   # Chargement, nettoyage, export des données
└── 02_eda.ipynb             # Analyse exploratoire et visualisations
data/
├── raw/                     # Données sources (non incluses — voir ci-dessous)
└── processed/               # Fichiers parquet nettoyés (non inclus)
reports/
└── LFB_DAB_Fev26_Rapport_Final_Gaetan_Seynave.pdf
 
---

## Tableau de bord Power BI

[![Power BI](https://img.shields.io/badge/Power%20BI-Rapport%20Interactif-F2C811?style=for-the-badge&logo=powerbi)](https://app.powerbi.com/view?r=eyJrIjoiZTcwYzVlZTUtZDZmYS00YjQwLWIxODEtMjUxYTkwZDU4MzlkIiwidCI6IjI3YThmZjFkLTc1YTAtNGFlNC1hNTg2LTMxN2NlOWVhYWZmYiJ9)

Le dashboard couvre 3 axes : état de la situation, cartographie des incidents, 
et analyse de la performance par rapport aux objectifs légaux.

---

## Données sources

Les données sont publiques et téléchargeables sur le
[London Data Store](https://data.london.gov.uk/) :
- [Incident Records](https://data.london.gov.uk/dataset/london-fire-brigade-incident-records-em8xy/)
- [Mobilisation Records](https://data.london.gov.uk/dataset/london-fire-brigade-mobilisation-records-24r65/)

Les fichiers ne sont pas inclus dans ce repo (trop volumineux — environ 1,5 Go au total).
Une fois téléchargés, les placer dans `data/raw/` et lancer `01_preprocessing.ipynb`.

---

## Stack technique

Python 3.12 · pandas · numpy · matplotlib · seaborn · pyproj  
Power BI Desktop (via Parallels sur Mac)  
Données météo : API Open-Meteo

---

## À propos

Fort d'une solide compréhension business et d'une expérience data concrète en entreprise,
je me repositionne comme Data Analyst avec une double compétence métier/technique :
capable de traduire un besoin business en analyse actionnable, et de le mener
de bout en bout — du preprocessing au tableau de bord.

[LinkedIn](https://www.linkedin.com/in/gaetan-seynave)
