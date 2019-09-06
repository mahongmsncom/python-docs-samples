# Getting started with Django on Google Cloud Platform on App Engine Standard

[![Open in Cloud Shell][shell_img]][shell_link]

[shell_img]: http://gstatic.com/cloudssh/images/open-btn.png
[shell_link]: https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/GoogleCloudPlatform/python-docs-samples&page=editor&open_in_editor=appengine/standard/django/README.md

This repository is an example of how to run a [Django](https://www.djangoproject.com/) 
app on Google App Engine Standard Environment. It uses the 
[Writing your first Django app](https://docs.djangoproject.com/en/1.9/intro/tutorial01/) as the 
example app to deploy.


# Tutorial
See our [Running Django in the App Engine Standard Environment](https://cloud.google.com/python/django/appengine) tutorial for instructions for setting up and deploying this sample application.

# Local Setup
#### - https://cloud.google.com/python/django/appengine
- pyenv virtualenv 2.7.16 doc-django-s27
- pip install -r requirements.txt
- ```
    python manage.py makemigrations
    python manage.py makemigrations polls
    python manage.py migrate
  ```
- python manage.py createsuperuser
- super: mahong, pwd: mh123456
- python manage.py runserver 5001
- http://localhost:5001/admin

# Deploy on GAE Standard
- pip install -t lib/ PyMySQL==0.9.2

- gcloud config configurations list
- gcloud config configurations activate mh001
- gcloud info