# Symfony Docker (PHP8 / Node20 / Mysql8)

A [Docker](https://www.docker.com/)-based installer and runtime for the [Symfony](https://symfony.com) web framework, with HTTPS support.

## Getting Started

1. If not already done, install Docker Desktop
2. Run `docker compose -f docker-compose.dev.yml up` to build the project or Run `docker compose -f docker-compose.dev.yml up -d` to run in background
3. Open `https://localhost` in your favorite web browser.
4. Run `docker compose -f docker-compose.dev.yml logs -f` to display current logs, `docker compose -f docker-compose.dev.yml logs -f [CONTAINER_NAME]` to display specific container's current logs

## Commandes utiles
Lister l'ensemble des commandes existances `docker compose exec php bin/console`

#### Création de fichier vierge
Controller `docker compose exec php symfony console make:controller`

FormType `docker compose exec php symfony console make:form`

CRUD `docker compose exec php symfony console make:crud`

#### Debug
Supprimer le cache du navigateur

`docker compose exec php symfony console cache:clear`

`docker compose exec php symfony console c:c`

Voir les routes actives

`docker compose exec php symfony console debug:router`
