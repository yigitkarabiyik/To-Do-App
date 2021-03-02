{% if False %}

# To Do App

The goal of this project is to provide minimalistic django to do app project that some practice where came from cleverprogrammer youtube channel. 

Template is written with django 3.1 and python 3 in mind.

![Default Home View](static/__screenshots/home.png?raw=true "Title")

### Main features

* Bootstrap static files included

* Procfile for easy deployments

* Separated requirements files

* SQLite by default if no env variable is set

# Usage

To use this template to start your own to do app project:

### Existing virtualenv

If your project is already in an existing python3 virtualenv first install django by running

    $ pip install django
    
And then run the `django-admin.py` command to start the new project:

    $ django-admin.py startproject \
      --template=https://github.com/yigitkarabiyik/to_do_app.git \
      --extension=py,md \
      to_do_app
      
### No virtualenv

This assumes that `python3` is linked to valid installation of python 3 and that `pip` is installed and `pip3`is valid
for installing python 3 packages.

Installing inside virtualenv is recommended, however you can start your project without virtualenv too.

If you don't have django installed for python 3 then run:

    $ pip3 install django
    
And then:

    $ python3 -m django startproject \
      --template=https://github.com/yigitkarabiyik/to_do_app.git \
      --extension=py,md \
      to_do_app
      
      
After that just install the local dependencies, run migrations, and start the server.

{% endif %}

# {{ project_name|title }}

# Getting Started

First clone the repository from Github and switch to the new directory:

    $ git clone https://github.com/yigitkarabiyik/to_do_app.git
    $ cd {{ to_do_app }}
    
Activate the virtualenv for your project.
    
Install project dependencies:

    $ pip install -r requirements.txt
    
    
Then simply apply the migrations:

    $ python manage.py migrate
    

You can now run the development server:

    $ python manage.py runserver
    
https://kaskas-to-do-app.herokuapp.com/
