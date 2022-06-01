# django-base

This is base Django project to help kickstart new webapp.

## How to Setup Project

### 1. Clone the repo
```
git clone git@github.com:kishan/django-base.git
```

### 2. Create your own virtual environment
  ```
 $ python3 -m venv venv
 $ source venv/bin/activate
```

### 3. Install requirements
`$ pip install -r requirements.txt`

### 4. Set environment variables
Create `.env` file based upon `.env_sample` and fill in variables
```
cp .env_sample .env
```
`DJANGO_SECRET_KEY`: you'll need to generate new secret key. Can use [Djecrety](https://djecrety.ir/) to quickly generate secure secret keys.

### 5. Run server
We'll be using [localhost.run](localhost.run) which provides us with a publicly accessible URL to our Django app.
```
  $ python manage.py runserver
  $ ssh -R 80:localhost:8000 localhost.run
```
