# AiBetExpert

# AiBetExpert

AiBetExpert est une application innovante de paris sportifs qui utilise l'intelligence artificielle pour faciliter et améliorer la recherche de matchs intéressants sur lesquels parier. Grâce à des algorithmes avancés de traitement du langage naturel, AiBetExpert permet aux utilisateurs de trouver facilement les meilleures opportunités de paris en temps réel.

## Fonctionnalités

- Affichage en temps réel des résultats des matchs de football.
- Consultation des cotes des rencontres en direct.
- Recherche intelligente des matchs basée sur des critères définis par l'utilisateur.
- Utilisation de l'intelligence artificielle pour interpréter les requêtes en langage naturel.

## Technologies Utilisées

### Backend

- **Java** : Langage de programmation principal.
- **Spring Boot** : Framework pour construire des applications Java robustes et performantes.
- **PostgreSQL** : Base de données relationnelle pour stocker les données des matchs et des cotes.
- **Redis** : Cache pour améliorer la rapidité des requêtes.
- **Apache Kafka** : Message broker pour la gestion des flux de données en temps réel.
- **Elasticsearch** : Moteur de recherche pour des requêtes rapides et avancées.
- **Spring Security** : Sécurisation des accès à l'application.
- **Docker** : Conteneurisation des services pour un déploiement facile.
- **Kubernetes** : Orchestration des conteneurs pour la gestion des déploiements à grande échelle.
- **Prometheus et Grafana** : Monitoring et alerting des performances de l'application.

### Frontend

- **Angular** : Framework pour construire des interfaces utilisateur dynamiques et réactives.

### Intelligence Artificielle

- **Hugging Face Transformers** : Bibliothèque pour le traitement du langage naturel.
- **spaCy** : Bibliothèque NLP pour l'analyse et l'interprétation des requêtes utilisateur.
- **TensorFlow Serving** : Déploiement des modèles de machine learning.

## Prérequis

- **Java 11** ou supérieur.
- **Node.js** et **npm**.
- **Docker** et **Docker Compose**.
- **PostgreSQL**.
- **Redis**.
- **Elasticsearch**.
- **Kafka**.
- **Python 3.7** ou supérieur (pour l'IA).

## Installation

### Backend

1. Clonez le dépôt :
    ```sh
    git clone https://github.com/votre-utilisateur/BetIntelIA.git
    cd BetIntelIA/backend
    ```

2. Configurez les propriétés de l'application dans `src/main/resources/application.yml` :
    ```yaml
    spring:
      datasource:
        url: jdbc:postgresql://localhost:5432/aibetexpert
        username: votre-utilisateur
        password: votre-mot-de-passe
      jpa:
        hibernate:
          ddl-auto: update
    ```

3. Construisez et lancez l'application :
    ```sh
    ./mvnw clean install
    ./mvnw spring-boot:run
    ```

### Frontend

1. Déplacez-vous dans le répertoire frontend :
    ```sh
    cd ../frontend
    ```

2. Installez les dépendances :
    ```sh
    npm install
    ```

3. Lancez l'application Angular :
    ```sh
    ng serve
    ```

### Conteneurisation

1. Assurez-vous que Docker et Docker Compose sont installés.
2. Dans le répertoire racine du projet, lancez les services :
    ```sh
    docker-compose up --build
    ```

## Utilisation

- Accédez à l'application via `http://localhost:4200` pour le frontend.
- Les APIs backend seront disponibles via `http://localhost:8080`.

## Contribution

1. Forkez le projet.
2. Créez votre branche de fonctionnalité (`git checkout -b feature/nom-fonctionnalité`).
3. Commitez vos modifications (`git commit -m 'Ajout d'une fonctionnalité'`).
4. Poussez votre branche (`git push origin feature/nom-fonctionnalité`).
5. Ouvrez une Pull Request.

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.
