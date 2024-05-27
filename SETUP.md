# Set up

## Setting up for Django

1. Set Virtual environment.
2. $> Django_admin startproject funding
3. $> cd funding
4. $> code .
5. $> python manage.py startapp eventers

## Inside funding

### settings.py

INSTALLED_APPS = [
    *add* 'eventers',
    *add* 'funders',
    *add* 'SignUp/Login/Logout ',
]
___________________

### urls.py

from django.urls import include, path

urlpatterns = [

    path(..............)

    path("eventers/", include("eventers.urls"))
]
