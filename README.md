# Django-Telegram Bot Template
Empty project for Django-Telegram-bot.

Use Django as usual

Use bot as command of Django

## Install
0. Use virtual environment
1. Create `.env` from `.env.Exmaple`
2. `pip install -r requirements.txt`

## .env
1. `TELEGRAM_TOKEN` - str, Get token from [BotFather](https://t.me/botfather)
2. `SECRET_KEY` - str, Django SECRET_KEY. Use console:`python manage.py shell -c 'from django.core.management import utils; print(utils.get_random_secret_key())'`
3. `DEBUG` - bool, Django mode
4. `ALLOWED_HOSTS` - list, Your hosts: `['.localhost', '127.0.0.1', '[::1]', '.herokuapp.com']`
5. `DATABASE_URL` - DB connection settings [example](https://github.com/jacobian/dj-database-url#url-schema)

## Run
### Bot
```
python manage.py migrate
python manage.py bot
```
### Django admin
### First run
```
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
http://127.0.0.1:8000/admin/
```
### Common run
```
python manage.py migrate
python manage.py runserver
```