<p align="center"><a href="https://540deg.com" target="_blank"><img src="https://pbs.twimg.com/profile_images/626765331357413376/p6BePNV1_400x400.jpg" width="200"></a></p>

Laravel docker

The project must be mounted using docker:

- Start docker daemon

- Run your docker machine: docker-compose up -d
- From inside the machine:
  - Run: composer install
  - Copy the .env.example to .env
  - Run: php artisan key:generate
- Web running on http://localhost:8088
- Api status check running on GET request: http://localhost:8088/api/status
- Swagger running on http://localhost:8082/
- Postman base collection file can be found on src/postman
- phpMyAdmin running on http://localhost:9191
  - user: root
  - password: secret
- As database we use MySQL:
  - database name: laravel
  - database user: root
  - database password: secret



- To stop de container:
  docker-compose stop

:)