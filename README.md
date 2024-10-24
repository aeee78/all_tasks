# taski-docker
## Описание
Веб-приложение для планирования своих задач. Задачи можно можно добавлять, удалять, отмечать завершенными и изменять.
## Технологии:

- Python
- PostgreSQL
- Django
- Django REST Framework
- Nginx
- Docker
- GitHub Actions

## Запуск приложения в Docker

1. Клонируйте репозиторий:
2. В корне проекта переименуйте файл `.env.example`, в `.env`.
3. Запустите Docker контейнеры:
   ```bash
   docker-compose up -d
   ```
4. Выполните миграции и создайте суперпользователя:
   ```bash
   docker-compose exec backend python manage.py migrate
   docker-compose exec backend python manage.py createsuperuser
   docker-compose exec backend python manage.py collectstatic --no-input
   ```
