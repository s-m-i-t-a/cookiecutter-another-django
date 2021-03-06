cookiecutter-another-django
===========================

.. image:: https://requires.io/github/s-m-i-t-a/cookiecutter-another-django/requirements.svg?branch=master
    :target: https://requires.io/github/s-m-i-t-a/cookiecutter-another-django/requirements/?branch=master
    :alt: Requirements Status

A cookiecutter_ template for Django.

.. _cookiecutter: https://github.com/audreyr/cookiecutter

Features
---------

* Django 1.7
* Twitter Bootstrap 3
* Registration via django-allauth
* User avatars via django-avatar
* Procfile for deploying to Heroku
* Heroku optimized requirements
* Basic caching setup
* Use pytest

Constraints
-----------

* Only maintained 3rd party libraries are used.
* PostgreSQL everywhere
* Environment variables for configuration (This won't work with Apache/mod_wsgi)

Usage
------

Let's pretend you want to create a Django project called "redditclone". Rather than using `startproject`
and then editing the results to include your name, email, and various configuration issues that always get forgotten until the worst possible moment, get cookiecutter_ to do all the work.

First, get cookiecutter. Trust me, it's awesome::

    $ pip install cookiecutter

Now run it against this repo::

    $ cookiecutter https://github.com/s-m-i-t-a/cookiecutter-another-django.git

You'll be prompted for some questions, answer them, then it will create a Django project for you.


**Warning**: After this point, change 'Jindřich Smitka', 'smitka.j', etc to your own information.

It prompts you for questions. Answer them::

    Cloning into 'cookiecutter-another-django'...
    remote: Counting objects: 550, done.
    remote: Compressing objects: 100% (310/310), done.
    remote: Total 550 (delta 283), reused 479 (delta 222)
    Receiving objects: 100% (550/550), 127.66 KiB | 58 KiB/s, done.
    Resolving deltas: 100% (283/283), done.
    project_name (default is "project_name")? redditclone
    repo_name (default is "repo_name")? redditclone
    author_name (default is "Your Name")? Jindřich Smitka
    email (default is "Your email")? smitka.j@gmail.com
    description (default is "A short description of the project.")? A reddit clone.
    year (default is "Current year")? 2013
    domain_name (default is "Domain name")?


Enter the project and take a look around::

    $ cd redditclone/
    $ ls

Create a Bitbucket repo and push it there::

    $ git init
    $ git add .
    $ git commit -m "first awesome commit"
    $ git remote add origin git@bitbucket.org:jsmitka/redditclone.git
    $ git push -u origin master

Now take a look at your repo. Awesome, right?

It's time to write the code!!!


"Your Stuff"
-------------

Scattered throughout the Python and HTML of this project are places marked with "your stuff". This is where third-party libraries are to be integrated with your project.


Not Exactly What You Want?
---------------------------

This is what I want. *It might not be what you want.* Don't worry, you have options:

Fork This
~~~~~~~~~~

If you have differences in your preferred setup, I encourage you to fork this to create your own version.

Or Submit a Pull Request
~~~~~~~~~~~~~~~~~~~~~~~~~

I also accept pull requests on this, if they're small, atomic, and if they make my own project development
experience better.
