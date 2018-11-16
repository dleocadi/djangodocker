# Project Title

Docker project to create a Django container and Postgres DB

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

## Prerequisites

Docker & Docker Compose

## Run these commands to create and run the containers

            docker-compose run web django-admin.py startproject djrepo .

Edit DATABASE configuration in this file djrepo/settings.py with:
            
            DATABASES = {
                        'default': {
                            'ENGINE': 'django.db.backends.postgresql_psycopg2',
                            'NAME': 'postgres',
                            'USER': 'postgres',
                            'HOST': 'db',
                            'PORT': 5432,
                        }
            }


To start the containers run:
            
            docker-compose up

Access the Django container at:
            
            http://localhost:8000

## Authors
Daniel Leocadi
See also the list of contributors who participated in this project.

## License
This project is licensed under the MIT License - see the LICENSE.md file for details
