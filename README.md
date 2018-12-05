# Docker Nginx, Laravel, MySQL

## Installation
```
1. Run docker network create web-proxy
2. Change your timezone in file web > Dockerfile line 10
3. Copy file .env.example to .env in folder web > www (cp .env.example .env)
4. Chmod folder web > www > storage to 777 (chmod 777 -R storage)
5. Run docker-compose up -d
6. Run docker-compose exec web composer install
7. Run docker-compose exec web php artisan key:generate
8. Need migrate data ? Setting your .env in folder web > www and then docker-compose exec web php artisan migrate 
9. Happy coding :)
```
