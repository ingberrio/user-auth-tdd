# user-auth-tdd 🥷🏻
TDD user interface with django

# Tecnologies 🧑🏻‍🚀
Django>=4.0.4,<4.1

djangorestframework>=3.13.1,<3.14

psycopg2>=2.9.3,<2.10

Flake8

Docker version 20.10.17

# Commands 🧑🏻‍💻
docker-compose run --rm app sh -c "python manage.py makemigrations"

docker-compose run --rm app sh -c "python manage.py migrate"

docker-compose build

docker-compose up

# Test 🦸🏼
docker-compose run --rm app sh -c "python manage.py test"

docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py test && flake8"
