# First django project - should be a snipped for the next one

## Instalation

**Pipenv**

``` 
pipenv shell
```

**django**
 
```
$ pipenv install django
```

**DB - default is SQLite - stick at first**

## Command lines

**Start project**

- `$ django-admin startproject <NAME>` — NAME — is a project name, you can create as many projects as you need

**Start server**

- `$ python manage.py runserver PORT` - if port not set 8000
-- after first run message about unapplied migration(s)


## Core files

- The most important is `manage.py` file in the project directory — the hart of the project for migration, installing etc.

- For managing the project adding new staff, arranging project inside the project find `settings.py` - file to arrange middleware, DB, KEY etc...

- Routs is place in `urls.py`

