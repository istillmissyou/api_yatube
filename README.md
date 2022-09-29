## What is this project about?

This project is an api for Yatube.

### How to launch a project:

Clone the repository and go to it on the command line:

``
the scoundrel is cloning https://github.com/istillmissyou/api_yatube .git
```

``
cd api_final_yatube
```

Create and activate a virtual environment:

``
python3 -m venv env
```

``
source env/bin/activate
```

`
python3 -m pip install --update pip
```

Install dependencies from a file requirements.txt:

``
installing pip -r requirements.txt
``

Perform migrations:

`
python3 manage.py migrate
```

Launch a project:

```
python3 manage.py startup server
```

### Requests

* api/v1/jwt/create/ (POST): we pass the username and password, we get the JWT token.
* api/v1/jwt/refresh/ (POST): updating the JWT token.
* api/v1/jwt/verify/ (POST): checking the JWT token.
* api/v1/posts/ (GET, PUBLISH): get a list of all messages or create a new message.
* api/v1/posts/{post_id}/ (GET, PUT, FIX, DELETE): get, edit, or delete a message by ID.
* api/v1/groups/ (GET): get a list of all groups.
* api/v1/groups/{group_id}/ (GET): getting information about a group by ID.
* api/v1/posts/{post_id}/comments/ (GET, POST): get a list of all comments on a post with id=post_id or create a new one by specifying the ID of the post we want to comment on.
* api/v1/messages/{post_id}/comments/{comment_id}/ (GET, PUT, FIX, DELETE): get, edit, or delete a comment on the record ID with id=post_id.
* api/v1/follow/ (GET, POST): returns all subscriptions of the user who made the request, or the subscription of the user on whose behalf the request was made, to the user passed in the request body.

## Authors 
Danil Shtun
