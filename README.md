# API Final Yatube

API для проекта Yatube, который позволяет взаимодействовать с блогами, комментариями и подписками.

## Как запустить проект:

### Клонирование репозитория:

git clone https://github.com/SabinaDzh/api_final_yatube.git
cd api_final_yatube

### Cоздание и активирование виртуального окружения:

python -m venv env
source env/bin/activate

### Установка зависимостей из файла requirements.txt:

python -m pip install --upgrade pip
pip install -r requirements.txt

### Выполнение миграции:

python manage.py migrate

### Запуск проекта:

python manage.py runserver

## Примеры запросов:

### Получение списка постов
GET /api/v1/posts/

### Создание нового поста
POST /api/v1/posts/
Content-Type: application/json

{
  "text": "Ваш текст поста",
  "group": 1
}
### Получение списка комментариев к посту
GET /api/v1/posts/{post_id}/comments/

Автор проекта @SabinaDzh
