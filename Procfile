release: python manage.py migrate
web: gunicorn DjangoTelegramBot.wsgi --log-file=-
bot: python manage.py bot