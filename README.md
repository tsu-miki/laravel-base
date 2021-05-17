## Laravel×Docker環境構築
### 構築環境
2021/04/15 更新

・PHP:7.4

・Composer:1.10

・Nginx:1.18

・node：14.2

・MySQL:8.0

・（Laravel:8.x）

### Set up（Your project）
1. git clone https://github.com/tsuzuki-auk/Laravel_base.git
2. cd backend
3. Clone your project.
4. cd ../
5. cp .env.example .env
6. docker-compose up -d --build
7. docker-compose exec app bash
8. Please, set up your project.

### Set up（Laravel8.x）
1. git clone https://github.com/tsuzuki-auk/Laravel_base.git
2. docker-compose up -d --build
3. docker-compose exec app bash
4. composer create-project --prefer-dist "laravel/laravel=8.*" .
5. http://127.0.0.1:10080/