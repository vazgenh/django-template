# django-template

Install prerequisites
```sh
sudo apt-get install libpq-dev python-dev 
sudo pip install psycopg2 
sudo apt-get install postgresql postgresql-contrib
```

Create database
```sh
sudo su postgres 
create user vazgen;
create database test owner vazgen;
ALTER ROLE vazgen with PASSWORD ‘123’;
```

Run Django server
```sh
python manage.py migrate --settings=settings.base
python manage.py runserver --settings=settings.base
```
