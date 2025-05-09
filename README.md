# 📊 Analyse en Temps Réel des Avis Amazon

Ce projet a pour but de créer un système de traitement **en temps réel** des commentaires Amazon afin de déterminer leur **polarité** (positif, neutre, négatif), à l’aide d’un ensemble d’outils Big Data et Machine Learning : **Kafka, Spark, MongoDB, Docker, Flask**.

---

## 🧱 Architecture

- **Kafka** : Streaming des avis clients (producer/consumer)
- **Spark (PySpark)** : Traitement des flux et entraînement des modèles de ML
- **MongoDB** : Stockage des résultats de prédiction
- **Flask** : API Web pour affichage en ligne des prédictions (mode *online*)
- **Dashboard offline** : Visualisation globale à partir des données archivées
- **Docker** : Conteneurisation de tous les services pour un déploiement simplifié

---

## 🚀 Lancement du projet

> 📌 *À venir* : configuration complète via `docker-compose.yml`  
> Les instructions pour l’exécution et les dépendances seront ajoutées prochainement.

---

## 📁 Structure du projet

```bash
bigdata-amazon-reviews/
├── kafka/         # Scripts de publication Kafka (Producer)
├── spark/         # Scripts Spark Streaming pour la prédiction
├── api/           # Application Flask (prédictions en ligne)
├── dashboard/     # Tableau de bord offline pour visualisation globale
├── data/          # Données téléchargées depuis Kaggle
├── model/         # Modèles ML sauvegardés
├── docker/        # Dockerfiles & configurations par service
├── docker-compose.yml  # Orchestration de tous les conteneurs
├── requirements.txt    # Dépendances Python
└── README.md
