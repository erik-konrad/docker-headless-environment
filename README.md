# docker-headless-environment

for quick install run

```
docker compose up
```

Ports:
* http://localhost - Webserver (internal hostname: php-apache)
* http://localhost:8055 - Directus Backend (internal hostname: directus)
* http://localhost:8000 - phpmyadmin (internal hostname: phpmyadmin)
* http://localhost:8025 - mailhog (internal hostname: mailhog - smtp port: 1025)

Database:
```
 hostname: mariadb
 port: 3306
 db: db
 db user: db
 db password: db
 ```