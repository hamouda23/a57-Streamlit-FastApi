Projet Exam Stack

Ce projet met en place une architecture complète basée sur Docker Compose avec trois services : 
une base de données PostgreSQL, un backend Python et un frontend Streamlit.

Structure du projet
exam-stack/
│
├── docker-compose.yml
├── README.md
│
├── backend/
│   ├── Dockerfile
│   ├── app.py
│   └── requirements.txt
│
├── frontend/
│   ├── Dockerfile
│   ├── app.py
│   └── requirements.txt
│
└── volumes/
    └── pgdata/
Description des services

db : service PostgreSQL, stocke les données de l’application.

backend : API Python qui communique avec la base PostgreSQL via SQLAlchemy.

frontend : interface utilisateur (par exemple Streamlit) qui interagit avec le backend.

Lancement du projet

Dans le dossier principal exam-stack/, exécute :
docker-compose up --build
Le backend sera accessible sur : http://localhost:8000

Le frontend sera accessible sur : http://localhost:8501

Arrêt et nettoyage

Pour arrêter et supprimer les conteneurs ainsi que les volumes :
docker-compose down -v
