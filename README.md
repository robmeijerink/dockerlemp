# Docker LEMP stack

Simpele flexibele LEMP stack gemaakt met Docker containers.

## Installatie Docker (MacOS)

Het makkelijkste is om dit met Homebrew te installeren:

`brew install docker docker-machine docker-compose`

`docker-machine create --driver virtualbox default`

`docker-machine env default`

`eval "$(docker-machine env default)"`

## Start Containers

`docker-compose up -d`

## Stop Containers

`docker-compose stop`

## Verwijder / cleanup data

`docker-compose rm`