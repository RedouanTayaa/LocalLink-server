# LocalLink - Plateforme de mise en relation locale

## Description
LocalLink est une plateforme d'annuaire collaboratif offrant une API RESTful et une interface utilisateur moderne.

## Architecture

Le projet est structuré en plusieurs services conteneurisés :

### Services principaux
- **API** : Développée avec Symfony et FrankenPHP
- **Frontend** : Application Next.js avec rendu côté serveur
- **Base de données** : PostgreSQL
- **Registry** : Registry Docker privée pour les images

### Monitoring
- **Prometheus** : Collecte et stocke les métriques
- **Grafana** : Tableaux de bord de visualisation
- **Loki** : Agrégation des logs
- **Node Exporter** : Métriques système
- **cAdvisor** : Surveillance des conteneurs
- **Alloy** : Agent de télémétrie

## Prérequis

- Docker et Docker Compose
- WSL 2 (si vous êtes sous Windows)
- Git

## Accès aux services
- **Application** : http://localhost
- **Grafana** : http://localhost:3001
- **Prometheus** : http://localhost:9090
- **cAdvisor** : http://localhost:8080
- **Registry Docker** : http://localhost:5000

## Développement
### Structure des dossiers
- **/api** : Code source de l'API Symfony
- **/front** : Code source du frontend Next.js
- **/deploy** : Fichiers de déploiement Docker
- **/monitoring** : Configuration du monitoring
- **/registry** : Stockage du registry Docker