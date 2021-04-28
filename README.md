# Статус Workflow
![example workflow](https://github.com/bogatovad/yamdb_final/actions/workflows/yamdb_workflow.yaml.yml/badge.svg)
# api_yamdb
api_yamdb
### Описание
API для проекта Yatube
### Технологии
1. Python3
2. Django REST Framework
3. Docker
4. Postgesql
5. Nginx
### Установка docker
Установите Docker в свою систему следуя инструкциям документации
https://docs.docker.com/get-docker/
### Клонирование репозитория
Затем склонируйте репозиторий к себе на компьютер, выполнив команду
```git clone https://github.com/bogatovad/infra_sp2.git```
### Команды для запуска приложения
```docker-compose up```
### Команду для создания суперпользователя
```docker-compose exec web python manage.py createsuperuser```
#### Команда для выполнения миграций
```docker-compose exec web python manage.py migrate --noinput```
### Команда для сбора статики в одну папку
```docker-compose exec web python manage.py collectstatic --no-input```
### Заполнение базы тестовыми данными
Для этого сначала заполните базу небольшим количеством данных, например — через админку Django, а затем выполните команду
```docker-compose exec web python manage.py dumpdata > fixtures.json```
### Автор
Артем Богатов
