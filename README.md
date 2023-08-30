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

You can follow these steps to set up and run the project on your local machine.

#### Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7 or later is required (You can download Python from the official website:
https://www.python.org/downloads/)

#### Setting Up And Running The Server

1. Clone the repository

    ```shell
    git clone https://github.com/SSHshadow222/my-first-django.git
    cd my-first-django
    ```

2. Create and activate a virtual environment

    ###### Windows:
    
    ```shell
    > py -m venv .venv 
    > .venv\Scripts\activate.bat
    ```
    
    ###### Unix-Like:
    
    ```shell
    $ python -m venv .venv
    $ source .venv/bin/activate
    ```

3. Install dependencies

    ```shell
    cd src
    pip install -r requirements.txt
    ```

4. Configure the environment file

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
    
5. Finally, run the server

    ```shell
    $ python manage.py runserver
    ```
