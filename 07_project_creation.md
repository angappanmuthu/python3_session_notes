# Django Project Creation Steps

## **Creating workspace directory**

```bash
mkdir [workspace_name]
```

### Note : Make sure to if virtualenv is installed else run this command

```bash
pip3 install virtualenv
```

## **Creating Virtual Environment**

```bash
virtualenv --python=python3.8 [env_name]
```

## **Activating Environment**

- for linux and mac

```bash
    source [env_path]/bin/activate
```

- for windows

```bash
    source [env_path]/Script/Activate.ps1
```

## **Install django framework**

```bash
   pip3 install django
```

## **Creating Django Project**

```bash
   django-admin startproject [project_name]
```

## **Creating Application in Django Project**

```bash
   python3 manage.py startapp [app_name]
```

## __Config Application in Django Project__

* [project_name]/[project_name]/settings.py
* In installed application list, we should append the application name that we created.

`[project_name]/[project_name]/settings.py`

```python
  INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'api' # <----- [app_name]
]
```

## __Should migrate django project that will allow's to create some essential table for django framework__ 

```bash
   python3 manage.py makemigrations
   python3 manage.py migrate
```

## __makemigration__ command

`This command will create python file locally which consist of some essential schema defined in ORM format.`


## __migrate__ command

`This command will convert the ORM to SQL, that help's to create a schema over the table in database that is configured in our project`

## __To understand the migration file by run this command__

```bash
python3 manage.py sqlmigrate [app_name] [file_number]
```

## __Creating django model__


```python
from django.db import models

# Create your models here.
class User(models.Model):
    name = models.CharField(max_length=40,default='')
    age = models.IntegerField(default=0)

    def __str__(self):
        return str(self.name)

class Product(models.Model):
    name = models.CharField(max_length=40,default='')
    price = models.IntegerField(default=0)

    def __str__(self):
        return f'{self.id} [{self.name}] {self.price}'
```

- `Note : When ever we modify the model we should run this command to recognize the model that are defined in an app`

```bash
    python3 manage.py makemigrations
    python3 manage.py migrate
```

## __Django Admin Panel__

### __Register Model__

- It would register our models in django admin panel. 
- It help to do some essential features for admin user.
- That is basic curd operation of the models with UI (User Interface) and etc..


```python
from django.contrib import admin
from api.models import *

# Register your models here.

# admin.site.register(User)
# admin.site.register(Product)

# or

admin.site.register([User,Product])
```

### __Creating Super User__

- Creating super user to access an admin panel.


```bash
    python3 manage.py createsuperuser
```

- `localhost:8000/admin` to access admin panel.