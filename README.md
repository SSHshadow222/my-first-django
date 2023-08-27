# My Tennis Club 🎾

My Tennis Club is a web application used to represent some data
about the members of a tennis club. This is
my first-ever Django project and it was intended for learning
purposes only.

## Configuration

#### Middleware

* [WhiteNoise](https://whitenoise.readthedocs.io/en/latest/): Pip package
that allows web apps to serve their static files such as JavaScript, CSS,
and Images.

#### Database 

* [SQLite](https://www.sqlite.org/index.html): Embedded, serverless
relational database management system. 

## Installation

Follow these steps to set up and run the project on your local machine.

#### Prerequisites

Python 3.7 or later (You can download Python from the official website:
https://www.python.org/downloads/)

#### Clone The Repository

```shell
git clone https://github.com/SSHshadow222/my-first-django.git
cd my-first-django
```

#### Create and Activate a Virtual Environment

###### Windows:

```shell
> py -m venv .venv 
> .venv\Scripts\activate.bat
```

###### Unix Like:

```shell
$ python -m venv .venv
$ source .venv/bin/activate
```

#### Install dependencies

```shell
cd src
pip install -r requirements.txt
```

#### Configure The Environment File

Create a .env file in my_tenis_club and add a secret key:

```env
SECRET_KEY=your_secret_key
```

To generate a random secret key run the following commands:

```python
$ python manage.py shell

>>> from django.core.management.utils import get_random_secret_key
>>> print(get_random_secret_key())
```

#### Run The Server

```shell
$ python manage.py runserver
```
