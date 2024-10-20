# User Manager

## Backend

Бэк проекта выполнена на Python.
БД создана с использованием SQLAlchemy.
Нужен запущенный бэк для того, чтобы работал фронт.

### Models

2 сущности:

Admin:
*   id
*   email
*   hashedPW
*   users (relation with User)

User:
*   id
*   avatar
*   email
*   firstName
*   lastName
*   position
*   skills
*   adminId (relation with Admin)

## Frontend

Фронт сделан с использованием React.
Стиль каждого компонента модифицирован в .css.
Диаграмма навыков использует библиотеку Chart.js.

### Usage

### `git clone https://github.com/Alex5067/FastAPIManager.git src`
### `cd src/docker`
### `docker-compose up`

Сначала нужно создать администратора с адресом электронной почты и паролем на бэке, затем можно будет войти на фронт и увидеть всех пользователей из базы данных.\
Измените .env, чтобы изменить ветку и порты.\
Откройте [http://localhost:8000/docs](http://localhost:8000/docs), чтобы увидеть методы API.

Страница будет перезагружена, если будут сделаны изменения.\
Страница показывет все доступные CRUD операции для бэка.
Используйте "Try it out" для каждой операции(меняет database.db) или используйте Postman.


Oткройте [http://localhost:3000](http://localhost:3000), чтобы смотреть веб-форму, которая позволит проверять пользователей.
