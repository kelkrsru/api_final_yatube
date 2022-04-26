## Проект API для Yatube

### Сведения о проекте:

Проект предназначен для возможности публикации постов авторами с помощью API
методов. Это позволяет выполнить интеграцию данного проекта с любыми другими 
приложениями и программами.

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/kelkrsru/api_final_yatube.git
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv venv
```

```
source venv/bin/activate
```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```

### Описание API

Описание API методов проекта доступно по адресу: http://127.0.0.1:8000/redoc/


### Несколько примеров:

#### Получение всех постов:

```
http://127.0.0.1:8000/api/v1/posts/   GET query
```

#### Создание поста:

```
http://127.0.0.1:8000/api/v1/posts/   POST query
```

```
JSON body query
{
    "text": "string",
    "image": "string",
    "group": 0
}
```

### Автор:

Евгений Кириллов