# api_final_yatube

### About:

```
An API that allows authenticated users to create,
edit and delete posts on the YaTube social network,
as well as view and comment on other users posts
and subscribe to other authors.
```

### Tech:

```
Python
Django
REST API
Django ORM
SQLite
JWT
```

### How to start:

Clone repository:

```
git clone git@github.com:mvlbulankin/api_final_yatube.git
```

```
cd api_final_yatube
```

Create and activate virtual environment:

```
python3 -m venv env
```

* If you have Linux/macOS

    ```
    source env/bin/activate
    ```

* If you have windows

    ```
    source env/scripts/activate
    ```

```
python3 -m pip install --upgrade pip
```

Install requirements.txt:

```
pip install -r requirements.txt
```

```
cd yatube_api
```

Do migrate:

```
python manage.py makemigrations
```

```
python3 manage.py migrate
```

Start project:

```
python3 manage.py runserver
```

### Examples

* GET http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/

  ```
  {
      "id": 0,
      "author": "string",
      "text": "string",
      "created": "2019-08-24T14:15:22Z",
      "post": 0
  }
  ```

* POST http://127.0.0.1:8000/api/v1/jwt/create/

  ```
  {
      "username": "string",
      "password": "string"
  }
  ```

* Other possible requests can be viewed

  ```
  http://127.0.0.1:8000/redoc/
  ```