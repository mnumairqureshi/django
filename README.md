# django
1 - pip install whitenoise
2 – change 2 command in the project according to the link
http://whitenoise.evans.io/
3 – complete above process
4 - Make profile
5 - Pip install gunicorn
6 – requirement file through command  =:  pip freeze > requirements.txt 
7 – import os 
8 – in setting.py   add line 
STATIC_ROOT = os.path.join(BASE_DIR, 'static')

9 – in procfile 
release: python manage.py makemigrations --no-input
release: python manage.py migrate --no-input
web: gunicorn projectfile.wsgi
10 -  push on github throw command line
11 – login to Heroku link the repo of the project



Requirement file 
djangorestframework==3.11.2
dj-database-url==0.5.0
Django==2.0
django-heroku==0.3.1
gunicorn==20.0.4
psycopg2==2.8.6
python-dotenv==0.15.0
pytz==2021.1
whitenoise==5.2.0





django_heroku.settings(locals())






https://devcenter.heroku.com/articles/django-app-configuration
https://realpython.com/django-hosting-on-heroku/
