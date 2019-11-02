# ProductHunt-Clone-Django
This is a clone of the Product Hunt website made using Django, Bootstrap and JavaScript, deployed using Heroku. It uses django-heroku, gunicorn, Pillow and whitenoise for hosting on Heroku itself.

## Overview

This web application creates an online catalog for some products, where users can browse available products, upvote them, add new products and manage their accounts.

The main features that have currently been implemented are:

* There are models for products and users.
* Users can view list and detail information for products.
* Logged In Users can create, view and upvote models.
* Admin users can create and manage models.

### Resources Used:
<ul>
<li> <a href="https://devcenter.heroku.com/categories/working-with-django">Working with Django Docs at Heroku </a>
<li> <a href="https://docs.sentry.io/clients/python/integrations/#django">Sentry for Django</a>
</ul>

## Quick Start

To get this project up and running locally on your computer:
1. Set up the [Python development environment](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/development_environment).
   I recommend using a Python virtual environment.
1. Assuming you have Python setup, run the following commands (if you're on Windows you may use `py` or `py -3` instead of `python` to start Python):
   ```
   pip3 install -r requirements.txt
   python3 manage.py makemigrations
   python3 manage.py migrate
   python3 manage.py collectstatic
   python3 manage.py createsuperuser # Create a superuser
   python3 manage.py runserver
   ```
1. Open a browser to `http://127.0.0.1:8000/admin/` to open the admin site
1. Create a few test products to see the site in action.
1. Open tab to `http://127.0.0.1:8000` to see the main site, with your new objects.
