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

- `$ django-admin startproject <PROJECT_NAME>` — PROJECT_NAME — is a project name, you can create as many projects as you need

**Start server**

- `$ python manage.py runserver PORT` - if port not set 8000
- after first run message about unapplied migration(s)
- so in this case run `$ python manage.py migrate` - create all DB tables etc
- create first app: `python manage.py startapp APP_NAME` - as many app you need


## Core files

- The most important is `manage.py` file in the project directory — the hart of the project for migration, installing etc.

- For managing the project adding new staff, arranging project inside the project find `settings.py` - file to arrange middleware, DB, KEY etc...

- Routs is place in `urls.py`

## Develop project

**create model**
Edit models.py in apps file
**Edit settings.py in main project file**
Add APP_NAMEConfig line to the INSTALLED_APPS
**Create migration**
- `$ python manage.py makemigration APP_NAME` - create migrations folder and file inside
- finally `$ python manage.py migrate` - to migrate app
**Update database**
- `$python manage.py shell` - go into interactive mode with DB
- just like python interpreter make whatever you want
```python
from polls.models import Question, Choice
Question.objects.all()
```
