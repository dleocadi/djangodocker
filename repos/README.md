## Run these commands to create a Django container
## 1) docker-compose run web django-admin.py startproject djrepo .
## 2) Edit DATABASE configuration in this file djrepo/settings.py with:

DATABASES = {
            'default': {
                'ENGINE': 'django.db.backends.postgresql_psycopg2',
                'NAME': 'postgres',
                'USER': 'postgres',
                'HOST': 'db',
                'PORT': 5432,
            }
}

## 3) To start the containers run:  docker-compose up
## 4) Access Django at http://localhost:8000
