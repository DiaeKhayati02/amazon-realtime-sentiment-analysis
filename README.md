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

> Les instructions pour l’exécution :
```bash
docker-compose up --build
```
---

## 📁 Structure du projet

```bash
bigdata-amazon-reviews/
├── kafka/         # Scripts de publication Kafka et Scripts Spark Streaming pour la prédiction (Producer et Consummer )
├── data/         # Data et MongoLoader
├── Flask_app/           # Application Flask Tableau de bord offline pour visualisation globale
├── model/         # Modèles ML sauvegardés
├── utils/        # fonctions de preprocessing
├── Notebooks/        # entrainement de modeles
├── docker-compose.yml  # Orchestration de tous les conteneurs
├── requirements.txt    # Dépendances Python
└── README.md
```
📌 Features

Real-time ingestion and processing of Amazon reviews
Automated sentiment analysis using machine learning
Scalable, containerized microservices architecture
Interactive dashboards for both real-time and offline analytics
