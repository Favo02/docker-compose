## Docker compose

My docker files for my home server.

### Things to check

- all services contains:
  - `container-name`
  - `restart: unless-stopped`
  - `:latest` or explicit version tag
- all `docker-compose.yml` follows `TEMPLATE.yml` style
- all ports are in `.env`
- committed secrets in `.env` are only ports

### To Do

#### Use `.env` instead of hardcoded secrets

- express-socialnetworkformusic
- nginx-php-superunimia
- serve-react-favo02dev

#### Change credentials

- authelia
- mongo-database
- nginx-reverse-proxy
- pihole
- portainer
- postgresql-database
- teamspeak-server mariadb

#### Use registry hub (GitHub or DockerHub) instead of building container locally

- express-socialnetworkformusic
- nginx-php-superunimia
- serve-react-favo02
