# Домашнее задание к лекции «Docker»

## [Задание 1]

* Dockerfile в корне
* index.html приложен в отдельной папке html

#### Для теста использовал команды:
1. docker build . --tag=nginx_new_welcompage
2. docker run -d -p 8000:80 --rm nginx_new_welcompage
3. curl localhost:8000

## [Задание 2]

* Dockerfile в корне
* Папка проекта CRUD приложена
* БД изменена на SQLite и заполнена примерами
* Переменная окружения по умолчанию:
  * MyENV=Default

#### Для теста использовал команды:
1. docker build . --tag=crud_python
2. docker run -it crud_python
3. docker exec -it 1b29b941d185 bash
4. curl localhost:8000

#### REST API приложения:
1. *"/"* - страничка с выводом переменной окружения
2. *"/api/v1/stocks/"* - склады
3. *"/api/v1/products/"* - продукты


