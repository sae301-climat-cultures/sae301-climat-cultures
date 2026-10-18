# SAÉ 3.01 – Climat & Cultures (FLORA2050) · Groupe FA2

Rendu du jalon J1. Ce fichier décrit l'organisation de l'archive et indique quoi ouvrir selon ce que vous cherchez.

## Arborescence

```
Rendu/
├── README_sae301_FA2.md                         ← ce guide
├── docAnalyse_sae301_FA2.pdf                    ← document d'analyse complet
├── Data/
│   ├── referentielCultures_sae301_FA2.xlsx      ← seuils agronomiques par culture
│   └── dimensions_sae301_FA2.pdf                ← description des dimensions (modèle de données)
└── Dev/
    ├── Maquette/
    │   ├── maquette_sae301_FA2.pdf              ← maquette, toutes les vues
    │   └── justificationMaquette_sae301_FA2.pdf ← choix de conception de la maquette
    └── Appels Api/
        ├── compteRenduAppelsApi_sae301_FA2.pdf  ← explication des appels Open-Meteo
        └── serieMelun2049_sae301_FA2.json       ← réponse JSON d'un appel (Melun, 2049)
```

## Contenu

### Racine
- **docAnalyse_sae301_FA2.pdf** – Le point d'entrée. Cadrage du projet (contexte, besoin, objectifs, acteurs), fonctionnalités par priorité, architecture de l'application, MVP, backlog et critères de faisabilité.

### Data/
- **referentielCultures_sae301_FA2.xlsx** – Notre référentiel de seuils : une ligne par culture avec les seuils climatiques utilisés pour juger sa viabilité.
- **dimensions_sae301_FA2.pdf** – Le modèle de données : tables (cultures, caractéristiques, communes, données météo…), leurs attributs et leurs relations.

### Dev/Maquette/
- **maquette_sae301_FA2.pdf** – Toutes les vues de l'application : Accueil, Résultat, Bilan commune, Fiche culture, Compte.
- **justificationMaquette_sae301_FA2.pdf** – Pourquoi la maquette est construite ainsi : aspect global, navigation, choix visuels, affichage des limites des données.

### Dev/Appels Api/
- **compteRenduAppelsApi_sae301_FA2.pdf** – Premiers appels à l'API Open-Meteo : paramètres envoyés, modèles climatiques comparés, structure de la réponse, constats (temps de réponse, valeurs manquantes, incohérences) et fonctionnement du cache.
- **serieMelun2049_sae301_FA2.json** – Exemple de réponse : Melun, année 2049, températures min/moy/max et précipitations. Le bloc `meta` décrit la commune, la source, la période et les unités.

## Par où commencer

1. **docAnalyse** pour comprendre le projet.
2. **Data/** pour voir les données sur lesquelles reposent les verdicts.
3. **Dev/Maquette/** pour voir l'application, puis **Dev/Appels Api/** pour la récupération des données climatiques.

## Convention de nommage

Tous les fichiers suivent le format `nomDuFichier_sae301_FA2.extension`.
