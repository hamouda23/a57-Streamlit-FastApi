# Docker + Streamlit + FastAPI + PostgreSQL  
**Projet complet : Application de gestion de notes avec persistance**

[![Docker](https://img.shields.io/badge/Docker-Enabled-blue?logo=docker)](https://www.docker.com/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.30-red?logo=streamlit)](https://streamlit.io/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104-green?logo=fastapi)](https://fastapi.tiangolo.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-blue?logo=postgresql)](https://www.postgresql.org/)

---

## Description

Une **application full Docker** composée de :
- **Frontend** : [Streamlit](https://streamlit.io) (UI interactive)
- **Backend** : [FastAPI](https://fastapi.tiangolo.com) (API REST)
- **Base de données** : PostgreSQL (persistance via volume nommé)

Fonctionnalité principale :  
> **Ajouter des notes + Afficher la liste en temps réel + Persistance après redémarrage**

---

## Fonctionnalités

| Fonction | État |
|--------|------|
| Ajouter une note via formulaire | Done |
| Affichage dynamique de la liste | Done |
| Persistance des données (volume `pgdata`) | Done |
| Communication interne (`backend:8000`, `db:5432`) | Done |
| Healthcheck + `depends_on: service_healthy` | Done |
| Accès frontend via `localhost:8501` | Done |

---


