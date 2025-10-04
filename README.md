# 💰 Suivi du Chiffre d’Affaires (CA) – Cas réel en PME industrielle


## 🎯 **Objectif du projet**


Ce dashboard Power BI a été conçu pour offrir une vision claire et fiable du chiffre d’affaires réalisé, en intégrant les écritures comptables issues de Sage 100 et les factures de l’ERP Batigest.
L’objectif : permettre à la Direction et à la DAF de piloter le CA en temps réel, tout en suivant les encours clients et les retards de paiement.

---

## 🧠 **Contexte métier**


Avant ce projet, les équipes financières de l’entreprise devaient croiser manuellement les données issues de différents outils : Sage, Batigest et fichiers Excel.
La consolidation des chiffres prenait plusieurs jours et ne permettait pas d’avoir une vision fiable en cours de mois.
Le dashboard vise donc à :

Centraliser les sources comptables et ERP

Automatiser le calcul du CA et des encours

Garantir la cohérence entre les systèmes financiers et commerciaux

---

## 📊 **Fonctionnalités principales**


CA réel calculé automatiquement à partir des écritures comptables (débits / crédits)

Consolidation Sage + Batigest via connecteurs ODBC et clés de correspondance

Suivi des encours clients (réglés, échus, en cours)

Analyse temporelle par année fiscale, mois, trimestre, et commercial

Identification des avoirs et régularisations

DAX avancé pour le calcul des montants HT nets, cumuls et comparatifs N/N-1

Visualisations dynamiques : barres empilées, cartes de KPI, filtres temporels et sectoriels

---

## ⚙️ **Technologies utilisées**


Power BI Desktop

Power Query (ETL, nettoyage et modélisation)

DAX (calculs de CA, avoirs, retards, cumuls)

ODBC Sage 100 (intégration comptable automatisée)

Excel (fichiers auxiliaires, correspondances comptes et clients)

---

## 🧩 **Structure technique**


Modèle en étoile :

Table de faits FACT_F_ECRITUREC

Dimensions DIM_DATE, DIM_COMPTE_CLIENT, DIM_COMPTE_FOURNISSEUR

Jointures croisées entre Sage et Batigest pour associer les factures aux écritures

Calculs DAX pour les agrégations dynamiques et les écarts temporels

Catégorisation automatique des comptes produits (Atelier, Négoce, Pose, etc.)

---

## 🚀 **Résultats & impacts**


📈 Vision quotidienne du CA consolidé, sans retraitement manuel

⏳ Gain de temps pour la DAF sur les clôtures mensuelles

💡 Meilleure compréhension des encours et retards clients

🤝 Alignement des services financiers et commerciaux

🧭 Indicateur central pour le pilotage global de l’activité

---

## 📁 **Confidentialité**


Les données utilisées sont issues du système d’information interne et ne peuvent être diffusées publiquement (RGPD & confidentialité entreprise).
Ce projet illustre néanmoins un cas concret d’intégration comptable et analytique en PME industrielle.

---

## ✅ **En résumé**


Un projet complet combinant :

Intégration multi-sources (Sage + ERP)

Structuration de la donnée comptable

Automatisation Power BI

Fiabilisation du CA et des encours clients
