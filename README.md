# 💰 Suivi du Chiffre d’Affaires (CA) – Cas réel en PME industrielle

## 🎯 Objectif du projet


Ce dashboard Power BI offre une vision fiable et à jour du chiffre d’affaires (N / N-1 / N-2), en consolidant les écritures comptables (Sage 100) et les factures de l’ERP (Batigest).
Objectif : piloter la performance commerciale (mix FOURNI / FOURNI POSE, bureaux, clients) et suivre les encours (échu, réglé, en cours) sur année fiscale (avril → mars).



## 🧠 **Contexte métier**


Avant ce projet, les équipes naviguaient entre Sage, Batigest et Excel pour reconstituer le CA : perte de temps, incohérences, peu de vision à date.
Le dashboard apporte une source unique de vérité, automatise la consolidation et aligne DAF & Commerce sur les mêmes chiffres.



## 📊 **Fonctionnalités principales**


- Courbe CA N / N-1 / N-2 (mensuel & YTD) + variations (€ / %)

- Mix d’activité : répartition FOURNI vs FOURNI POSE (global + évolution mensuelle)

- Bureaux / Représentants : % du CA, tendance par mois, comparatif

- Clients : top clients, évolution mensuelle, contribution au CA

- Encours clients : statut réglé / échu / en cours, jours de retard calculés

- Filtres : année fiscale, mois, bureaux, clients, type de vente



## ⚙️ **Technologies utilisées**


- Power BI Desktop

- Power Query (ETL, nettoyage et modélisation)

- DAX (calculs de CA, avoirs, retards, cumuls)

- ODBC Sage 100 (intégration comptable automatisée)

- Excel (fichiers auxiliaires, correspondances comptes et clients)



## 🧩 **Structure technique**


Modèle en étoile :

- FACT_CA (écritures + factures consolidées, avoirs nettes)

- DIM_DATE (fiscal : avril → mars, Y, Q, M, YTD)

- DIM_CLIENT, DIM_BUREAUX (dérivé des représentants)

- DIM_TYPE_FACTURE (FOURNI / FOURNI POSE) & DIM_COMPTE_PRODUIT

Règles métiers :

- Normalisation débit/crédit → montant HT net (avoirs négatifs)

- Mapping Grp1 → FOURNI / FOURNI POSE

- Attribution Bureaux depuis CodeRepre

- Jointure Sage ↔ Batigest par numéro de facture

- Encours & retards calculés depuis dates d’échéance (conditions de règlement)



## 🚀 **Résultats & impacts**


📈 Vision quotidienne du CA consolidé, sans retraitement manuel

⏳ Gain de temps pour la DAF sur les clôtures mensuelles

💡 Meilleure compréhension des encours et retards clients

🤝 Alignement des services financiers et commerciaux

🧭 Indicateur central pour le pilotage global de l’activité



## 📁 **Confidentialité**


Les données utilisées sont issues du système d’information interne et ne peuvent être diffusées publiquement (RGPD & confidentialité entreprise).
Ce projet illustre néanmoins un cas concret d’intégration comptable et analytique en PME industrielle.



## ✅ **En résumé**


Un projet complet combinant :

Intégration multi-sources (Sage + ERP)

Structuration de la donnée comptable

Automatisation Power BI

Fiabilisation du CA et des encours clients
