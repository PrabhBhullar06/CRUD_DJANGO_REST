# CRUD_DJANGO_REST

Follow the steps to setup the project:
1. git clone https://github.com/PrabhBhullar06/CRUD_DJANGO_REST.git
2. cd CRUD_DJANGO_REST/
3. virtualenv --python='which python3' venv
4. source venv/bin/activate
5. pip install  Django==2.0.2
                djangorestframework==3.7.7
                psycopg2==2.7.3.2
6. cd myproject
7. cd myproject and open settings.py and make following changes to DATABASES SETTINGS(to change the database to postgresql):
   'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': 'djangodb', #Name of your postgresql database
        'USER': 'todoapp',  #username generated
        'PASSWORD':'mypassword',  #password generated
        'HOST': 'localhost',
        'PORT': '5433',
    }  
8. python manage.py makemigrations
9. python manage.py migrate
10. python manage.py runserver


Application will start at:
For web view: 127.0.0.1:8000
For JSON REST view: 127.0.0.1:8000/api
                
