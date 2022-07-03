## What is the project about?

This project is api for Yatube.

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/api_final_yatube.git
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

```
source env/bin/activate
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

### Requests

* api/v1/api-token-auth/ (POST): we pass the username and password, we get the token.
* api/v1/posts/ (GET, POST): get a list of all posts or create a new post.
* api/v1/posts/{post_id}/ (GET, PUT, PATCH, DELETE): get, edit or delete a post by id.
* api/v1/groups/ (GET): get a list of all groups.
* api/v1/groups/{group_id}/ (GET): get information about the group by id.
* api/v1/posts/{post_id}/comments/ (GET, POST): get a list of all post comments with id=post_id or create a new one by specifying the id of the post we want to comment on.
* api/v1/posts/{post_id}/comments/{comment_id}/ (GET, PUT, PATCH, DELETE): get, edit or delete a comment by the id of a post with id=post_id.

##### dev Danil Shtun

