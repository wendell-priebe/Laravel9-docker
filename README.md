## Modelo de exemplo do laravel com docker pronto.

### Como rodar:
Clonar repositório
```sh
git clone https://github.com/wendell-priebe/Laravel9-docker.git
```
Criar aquivo .env
```sh
cp .env.example .env
```
Altera campos do .env

![image](https://user-images.githubusercontent.com/61431715/157150667-9d6d49b7-9fe8-4a79-aae2-69441a966c43.png)
![image](https://user-images.githubusercontent.com/61431715/157150861-9fe29c50-1eaf-46ad-842b-95b61e1abf6b.png)
![image](https://user-images.githubusercontent.com/61431715/157150884-2ee002ea-fdf4-4d83-b406-475bb2ee7d41.png)


Criar containers
```sh
docker-compose up -d
```
Acessar container do PHP
```sh
docker-compose exec app bash
```
Instalar dependencias
```sh
composer install
```
Gerar chave key no .env
```sh
php artisan key:generate
```

Acessar: http://localhost:8080/
