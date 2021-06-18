# Статус Workflow
![example workflow](https://github.com/bogatovad/yamdb_final/actions/workflows/yamdb_workflow.yaml/badge.svg)
# api_yamdb
api_yamdb
### Описание
Проект собирает отзывы пользователей на произведения. Произведения делятся на категории: «Книги», «Фильмы», «Музыка». В каждой категории есть произведения: книги, фильмы или музыка. Произведению может быть присвоен жанр из списка предустановленных. Читатели оставляют к произведениям текстовые отзывы и выставляют произведению рейтинг (оценку в диапазоне от одного до десяти). Из множества оценок автоматически высчитывается средняя оценка произведения.
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
