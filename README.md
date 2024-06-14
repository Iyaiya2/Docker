# Application Node.js avec Docker

## Description

Ce projet montre comment mettre en conteneur une application Node.js simple en utilisant Docker. L'application utilise Express.js pour afficher un message "Hello World".

## Prérequis

- Docker installé sur votre machine
- Node.js installé sur votre machine (pour le développement local)

## Installation

1. Clonez le repository :
    ```sh
    git clone https://github.com/votre-nom-utilisateur/node-docker-app.git
    cd node-docker-app
    ```

2. Construisez l'image Docker :
    ```sh
    docker build -t node-docker-app .
    ```

3. Exécutez le conteneur Docker :
    ```sh
    docker run -p 3000:3000 node-docker-app
    ```

4. Accédez à l'application dans votre navigateur à l'adresse `http://localhost:3000`.

## Utilisation de Docker Compose

Vous pouvez aussi utiliser Docker Compose pour construire et exécuter l'application :

1. Démarrez l'application avec Docker Compose :
    ```sh
    docker-compose up
    ```

2. Accédez à l'application dans votre navigateur à l'adresse `http://localhost:3000`.

## Structure du projet

- `app.js` : Le fichier principal de l'application
- `package.json` : Métadonnées et dépendances du projet
- `Dockerfile` : Instructions pour construire l'image Docker
- `docker-compose.yml` : Fichier de configuration pour Docker Compose
- `.dockerignore` : Fichiers et répertoires à ignorer lors de la construction de l'image Docker

