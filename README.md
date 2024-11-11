## RU
# tasks_manager

Этот проект - полнофункциональное приложение для управления задачами, созданное с использованием Django для бэкенда и React для фронтенда.

## Функции

- Создание, обновление и удаление задач
- Просмотр списка задач
- Редактирование деталей задачи в модальном окне
- REST API для управления задачами
- Контейнеризация с помощью Docker для удобного развертывания

## Структура проекта

```
.
├── backend
│   ├── api
│   │   ├── admin.py
│   │   ├── models.py
│   │   ├── serializers.py
│   │   └── views.py
│   ├── backend
│   │   ├── settings.py
│   │   ├── urls.py
│   ├── manage.py
│   ├── requirements.txt
│   └── Dockerfile
├── frontend
│   ├── public
│   │   ├── index.html
│   │   ├── manifest.json
│   ├── src
│   │   ├── components
│   │   │   ├── Task.js
│   │   │   ├── TaskEditModal.js
│   │   │   ├── TabList.js
│   │   ├── index.js
│   │   ├── App.js
│   ├── package.json
│   ├── Dockerfile
├── LICENSE
└── README.md
```

## Технологии:

- Python
- PostgreSQL
- Django
- Django REST Framework
- HTML/CSS
- Nginx
- Docker
- GitHub Actions

## Бэкенд

Бэкенд построен с использованием Django и Django REST framework.

### Установка

1. Перейдите в директорию `backend`:
    ```
    cd backend
    ```
2. Создайте виртуальное окружение и активируйте его:
    ```
    python -m venv venv
    ```
    ```
    source venv/bin/activate  # На Windows используйте `venv\Scripts\activate`
    ```
3. Установите зависимости:
    ```
    pip install -r requirements.txt
    ```
4. Примените миграции:
    ```
    python manage.py migrate
    ```
5. Запустите сервер разработки:
    ```
    python manage.py runserver
    ```

### Конечные точки API

- **GET /api/tasks/**: Получить список задач.
- **POST /api/tasks/**: Создать новую задачу.
- **GET /api/tasks/{id}/**: Получить конкретную задачу по ID.
- **PUT /api/tasks/{id}/**: Обновить конкретную задачу по ID.
- **DELETE /api/tasks/{id}/**: Удалить конкретную задачу по ID.

## Фронтенд

Фронтенд построен с использованием React и Bootstrap.

### Установка

1. Перейдите в директорию `frontend`:
    ```
    cd frontend
    ```
2. Установите зависимости:
    ```
    npm install
    ```
3. Запустите сервер разработки:
    ```
   npm start
     ```

## Docker

Чтобы запустить все приложение с использованием Docker:

1. Убедитесь, что Docker установлен и запущен на вашем компьютере.
2. Соберите и запустите контейнеры:
    ```sh
    docker-compose up --build
    ```

## Благодарности

- [Django](https://www.djangoproject.com/)
- [React](https://reactjs.org/)
- [Bootstrap](https://getbootstrap.com/)
- [Docker](https://www.docker.com/)

---
## EN
# tasks_manager

This project is a full-stack Task Management Application built using Django for the backend and React for the frontend.

## Features

- Create, update, and delete tasks
- View a list of tasks
- Edit task details in a modal
- REST API for task management
- Dockerized for easy deployment

## Project Structure

```
.
├── backend
│   ├── api
│   │   ├── admin.py
│   │   ├── models.py
│   │   ├── serializers.py
│   │   └── views.py
│   ├── backend
│   │   ├── settings.py
│   │   ├── urls.py
│   ├── manage.py
│   ├── requirements.txt
│   └── Dockerfile
├── frontend
│   ├── public
│   │   ├── index.html
│   │   ├── manifest.json
│   ├── src
│   │   ├── components
│   │   │   ├── Task.js
│   │   │   ├── TaskEditModal.js
│   │   │   ├── TabList.js
│   │   ├── index.js
│   │   ├── App.js
│   ├── package.json
│   ├── Dockerfile
├── LICENSE
└── README.md
```

## Technologies:

- Python
- PostgreSQL
- Django
- Django REST Framework
- HTML/CSS
- Nginx
- Docker
- GitHub Actions

## Backend

The backend is built with Django and Django REST framework.

### Setup

1. Navigate to the `backend` directory:
    ```
    cd backend
    ```
2. Create a virtual environment and activate it:
    ```
    python -m venv venv
    ```
    ```
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```
3. Install the dependencies:
    ```
    pip install -r requirements.txt
    ```
4. Apply the migrations:
    ```sh
    python manage.py migrate
    ```
5. Run the development server:
    ```sh
    python manage.py runserver
    ```

### API Endpoints

- **GET /api/tasks/**: Retrieve a list of tasks.
- **POST /api/tasks/**: Create a new task.
- **GET /api/tasks/{id}/**: Retrieve a specific task by ID.
- **PUT /api/tasks/{id}/**: Update a specific task by ID.
- **DELETE /api/tasks/{id}/**: Delete a specific task by ID.

## Frontend

The frontend is built with React and Bootstrap.

### Setup

1. Navigate to the `frontend` directory:
    ```
    cd frontend
    ```
2. Install the dependencies:
    ```
    npm install
    ```
3. Run the development server:
    ```
    npm start
    ```

## Docker

To run the entire application using Docker:

1. Make sure Docker is installed and running on your machine.

2. Build and run the containers:
    ```
    docker-compose up --build
    ```

## Acknowledgements

- [Django](https://www.djangoproject.com/)
- [React](https://reactjs.org/)
- [Bootstrap](https://getbootstrap.com/)
- [Docker](https://www.docker.com/)



