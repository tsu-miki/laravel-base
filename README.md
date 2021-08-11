## Laravel×Docker環境構築
### 構築環境
2021/07/16 更新

・PHP:7.4

・Composer:1.10

・Nginx:1.18

・node：14.2

・MySQL:8.0

・（Laravel:8.x）

### Set up（Your project）
1. git clone https://github.com/tsuzuki-auk/Laravel_base.git
2. git clone (your project) backend
3. cd backend
4. cp .env.example .env
5. docker-compose up -d
6. docker-compose exec app bash
7. composer install
8. php artisan key:generate
9. .env DB config set up
10. http://127.0.0.1:3000/
11. Please, set up your project.

### Set up（Laravel8.x）
1. git clone https://github.com/tsuzuki-auk/Laravel_base.git
2. mkdir backend
3. docker-compose up -d --build
4. docker-compose exec app bash
5. composer create-project --prefer-dist "laravel/laravel=8.*" .
6. http://127.0.0.1:3000/