### Start our image

```sh
docker-compose up
```
n
### Create superuser

```sh
docker-compose run --rm app python manage.py createsuperuser
```

### [Django Migrations](https://docs.djangoproject.com/en/4.0/topics/migrations/)
### If the command above fails to run, you might need to do an initial migration for the postgres database first:

```sh
docker-compose run --rm app python manage.py migrate
```