# Micro blog app in Flask

## To run

* Start pipenv shell session
* Ensure that you have the FLASK_DEBUG and FLASK_APP constants in the .flaskenv file
* python -m flask run
* To access the shell run: `flask shell`

## To Create Users

```
flask shell
>>> u = User(username='jonsnow', email='jon@snow.com')
>>> u.set_password('asdfasdf')
>>> db.session.add(u)
>>> db.session.commit()
```

## To run migrations

```
flask db migrate -m "Some migration message"
flask db upgrade
```

> Next: https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-vii-error-handling
