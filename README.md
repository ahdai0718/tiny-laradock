# Tiny Laradock

Fork from https://github.com/laradock/laradock, and keep it tiny.

## Service
  
  - `memcached`

  - `mysql`

  - `nginx`

  - `php-fpm`

  - `redis`

  - `td-agent`

## How to use

- `root`

  - `public`

  - `tiny-laradock`

    - Copy and rename `evn-example` to `.env`

    - Edit `.env`

      - `COMPOSE_PROJECT_NAME=`

      - `PHP_VERSION=`

    - Install `docker-compose`

      ```
      # curl -L https://github.com/docker/compose/releases/download/1.27.4/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose

      # chmod +x /usr/local/bin/docker-compose
      ```

    - `docker-compose`

      - `nginx`

        ```
        # docker-compose up -d --build nginx
        ```

      - `mysql`

        ```
        # docker-compose up -d --build mysql
        ```

      - `memcached`

        ```
        # docker-compose up -d --build memcached
        ```

      - 

        ```
        # docker-compose down
        ```