# PHP 8 Playground
A simple dockerized project for scaffolding new app written in PHP 8.

## Requirements
- Docker
- Docker-Compose

## Services
- PHP
- Nginx
- MariaDB

## Installation
```bash
# clone the project into your local computer
cd ~

git clone git@github.com:mrcyna/php8.git
cd php8

# create an env file
cp .env.example .env

# run containers via docker-composer
docker-compose up
```
Now you can confirm your installation by checking out the `http://127.0.0.1/` in your browser.

## CLI
to access PHP CLI you can run below command in your terminal:
```bash
docker-compose exec -u $(id -u ${USER}):$(id -g ${USER}) app bash
```

to access MariaDB CLI you can run below command in your terminal:
```bash
docker-compose exec mysql mysql -u root -p
```