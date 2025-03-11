# Aim of the tutorial

This tutorial walks you through the creation of a basic poll application.

It’ll consist of two parts:

- A public site that lets people view polls and vote in them.

- An admin site that lets you add, change, and delete polls.

# Install project

An informal overview of how to write a database-driven web app with Django.


To install project on a local machine run these commands:
```bash
$ python3 -m venv .venv
$ . .venv/bin/activate
(venv) $ pip install --upgrade pip
(venv) $ pip install -r requirements.txt
# (venv) $ python -m pip install Django
(venv) $ python manage.py runserver
# ...работает сервер, ctrl + c для выхода
(venv) $ deactivate
```

or simply run this script:
```
$ chmod +x install.sh (to change the permission settings of the files install.sh)
$ ./install.sh
```


# Create mysite (to bootstrap a new Django project)
(venv) $ mkdir djangotutorial
(venv)$ django-admin startproject mysite djangotutorial
(inside manage.py directory) python manage.py runserver
(inside manage.py directory) python manage.py startapp polls
$ python manage.py migrate
$ python manage.py makemigrations polls
$ python manage.py sqlmigrate polls 0001

New files are:

- manage.py: A command-line utility that lets you interact with this Django project in various ways. You can read all the details about manage.py in django-admin and manage.py.

- mysite/: A directory that is the actual Python package for your project. Its name is the Python package name you’ll need to use to import anything inside it (e.g. mysite.urls).

- mysite/__init__.py: An empty file that tells Python that this directory should be considered a Python package. If you’re a Python beginner, read more about packages in the official Python docs.

- mysite/settings.py: Settings/configuration for this Django project. Django settings will tell you all about how settings work.

- mysite/urls.py: The URL declarations for this Django project; a “table of contents” of your Django-powered site. You can read more about URLs in URL dispatcher.

- mysite/asgi.py: An entry-point for ASGI-compatible web servers to serve your project. See How to deploy with ASGI for more details.

- mysite/wsgi.py: An entry-point for WSGI-compatible web servers to serve your project. See How to deploy with WSGI for more details.

# Creating an admin user
$ python manage.py createsuperuser

# Run project
```
$ ./run.sh
```

and then  open your browser.

# TODO
- [x] TEXT
