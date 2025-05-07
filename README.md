<p align="center">
  <img src="docs/images/banner.png" alt="SmartAccess2030 Banner" width="700"/>
</p>

![Licence](https://img.shields.io/github/license/Hicham-Errihani/SmartAccess2030?style=for-the-badge&color=4caf50)
![Dernier commit](https://img.shields.io/github/last-commit/Hicham-Errihani/SmartAccess2030?style=for-the-badge&color=2196f3)
![Langage principal](https://img.shields.io/github/languages/top/Hicham-Errihani/SmartAccess2030?style=for-the-badge&color=ffeb3b)
![Taille du repo](https://img.shields.io/github/repo-size/Hicham-Errihani/SmartAccess2030?style=for-the-badge&color=ff9800)
![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-ready-2496ed?style=for-the-badge&logo=docker&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-Apache-black?style=for-the-badge&logo=apachekafka&logoColor=white)
![Spark](https://img.shields.io/badge/Spark-Streaming-f57c00?style=for-the-badge&logo=apachespark&logoColor=white)


---

## 🎯 Présentation du projet

### 🎫 **SmartAccess2030 — Système Intelligent de Gestion des Billets et du Public pour le Mondial 2030**

**SmartAccess2030** est une solution avancée de **gestion sécurisée des accès**, des **billets électroniques** et du **flux de spectateurs** pour les événements à très grande échelle, à commencer par la Coupe du Monde 2030.

Ce système innovant repose sur un pipeline technologique combinant **intelligence artificielle**, **Big Data**, et **traitement en temps réel**, afin d’optimiser la sécurité, l’organisation et l’expérience spectateur.

---

### 🚀 Fonctionnalités clés :

- 🎫 **Vérification rapide des billets numériques** (QR code, NFC, etc.)
- 🧠 **Reconnaissance faciale et vocale** pour authentification des détenteurs
- 📡 **Analyse temps réel des flux d’entrées** via **Kafka + Spark Streaming**
- 🔍 **Suivi des mouvements de foule** dans les stades via **capteurs et IA**
- 📊 **Tableaux de bord décisionnels** pour les organisateurs et les services de sécurité
- 📂 **Archivage complet** des sessions, accès, alertes et historiques de fréquentation

---

🎯 **Objectif principal** : assurer une gestion fluide, intelligente et ultra-sécurisée du public lors des matchs du **Mondial 2030**, tout en offrant aux organisateurs un outil de **pilotage temps réel**, de **détection de risques** et de **traçabilité complète**.

Ce projet répond aux standards des **grands événements internationaux**, dans une logique de **smart event**, **sécurité de masse**, et **expérience spectateur augmentée**.

---


---

## 🧱 Structure du projet

Le projet est structuré de manière modulaire, permettant une séparation claire entre les couches de traitement, d'authentification, de monitoring et de visualisation.

```bash
SmartAccess2030/
├── src/                  
│   ├── access_control/     🎟️  Authentification : QR, NFC, visage, voix
│   ├── ticketing/          🎫  Gestion des billets électroniques
│   ├── crowd_monitoring/   🧍‍♂️🧍‍♀️  Suivi et détection des foules
│   └── data_processing/    ⚙️  Nettoyage & transformation des flux de données
│
├── docker/                 🐳 Docker Compose (Kafka, Elastic, etc.)
├── data/                  
│   ├── raw/                📥 Données brutes (logs, entrées)
│   └── processed/          📤 Données préparées et enrichies
│
├── models/                 🧠 Modèles IA (facial, vocal, prédictions)
├── notebooks/              📓 Analyses exploratoires en Jupyter
├── docs/images/            🖼️ Bannières, schémas, captures d'écran
├── tests/                  ✅ Tests automatisés (API, sécurité, flux)
├── requirements.txt        📦 Dépendances Python du projet
└── README.md               📝 Documentation principale


---

---

## ⚙️ Installation & Lancement du Projet

> 🚀 Le projet peut être lancé en **local (Python)** ou via **Docker Compose**.  
> Voici les instructions pour les deux méthodes.

---

### 🔧 Prérequis

- ✅ Python 3.10 ou supérieur
- ✅ pip installé
- ✅ git installé
- 🐳 (optionnel) Docker & Docker Compose

---

### 🐍 Installation locale (avec environnement virtuel Python)

```bash
# 1. Cloner le dépôt
git clone git@github.com:Hicham-Errihani/SmartAccess2030.git
cd SmartAccess2030

# 2. Créer un environnement virtuel
python3 -m venv env

# 3. Activer l’environnement
source env/bin/activate       # Linux/macOS
# .\env\Scripts\activate       # Windows

# 4. Installer les dépendances
pip install -r requirements.txt

# 5. Lancer l'application (exemple)
cd src/
python app.py

