# Docker LEMP stack

Simpele LEMP stack gemaakt met Docker Compose.

- Nginx
- PHP
- MariaDB
- phpMyAdmin
- MailHog

Op zoek naar de <a href="https://github.com/robmeijerink/dockerlamp">LAMP</a> stack? Deze is vergelijkbaar, maar gebruikt Apache in plaats van Nginx en bevat ook meerdere PHP versies.

## Installatie Docker (MacOS)

Het makkelijkste is om dit met Homebrew te installeren:

`brew install docker docker-machine docker-compose`

`docker-machine create --driver virtualbox default`

`docker-machine env default`

`eval "$(docker-machine env default)"`

In de console zie je het ip adres waarmee je applicatie kunt bereiken in de browser.

Kopiëer nu alleen nog de `.env.example` naar `.env`.

## Start Containers

`docker-compose up -d`

## Stop Containers

`docker-compose stop`

## Sluit Containers af

`docker-compose down`

## Verwijder Containers

`docker-compose rm`

## Verwijder data uit volumes

Let op: hiermee verwijder je je databases.

`docker-compose rm -v`