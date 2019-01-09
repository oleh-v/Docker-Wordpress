# Docker. Wordpress - quick start
Quick start Wordpress environment with Docker

## Requirements
Docker and Docker-Compose should be installed
* [Docker ](https://docs.docker.com/install/) version 12 and above
* [Docker compose](https://docs.docker.com/compose/install/) version 1.10.0 and above

[Automatic installation Docker and Docker-Compose with Ansible ](https://github.com/oleh-v/Ansible-Docker-Install)

## Usage
* In docker-compose.yml (or stack.yml) file replace MYSQL_DATABASE, MYSQL_ROOT_PASSWORD, MYSQL_USER, MYSQL_PASSWORD with your own values
* To run the software, use:
```
docker-compose up -d
```

* ./db directory will contains database after creating
* ./www directory will contains wordpress site after creating


## Usage - SWARM mode:
* Swarm mode should be activated. If not - run command below:
```
docker swarm init
```
* Usage:
```
docker stack deploy -c stack.yml stack_name
```

* ./db directory will contains database after creating
* ./www directory will contains wordpress site after creating

## [Portainer](https://www.portainer.io/)
* [Portainer](https://www.portainer.io/) is a lightweight management UI which allows you to easily manage your different Docker environments (Docker hosts or Swarm clusters).
* Portainer will be available by accessing the port `9000` 