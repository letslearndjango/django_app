# django_app

## Set up

Install `brew`, the package manager for Mac OS.

```

```

Install `pyenv`, a python installation manager.

```
brew install pyenv
```

Install python version `3.6.7`, which also installs `virtualenv` and `pip`.

```
pyenv install 3.6.7
```

Switch to using `3.6.7`.

```
pyenv local 3.6.7
```

Install a virtual environment with `virtualenv`.

```
virtualenv venv --python=python3.6
```

Activate the virtual environment.

```
source venv/bin/activate
```

Install the python dependancies.

```
pip install -r requirements.txt
```

Start the development webserver.

```
django-admin runserver 0.0.0.0:8000
```

Point your web browser to `0.0.0.0:8000`.

```
open 0.0.0.0:8000
```

## Deployment

Install the heroku CLI.

```
brew install heroku
```

Log in to heroku.

```
heroku login
```

Ensure you have a git remote pointing to the right app.

```
heroku git:remote -a lld-django-app
```

Push to the heroku remote.

```
git push heroku
```

Once the changes have been built, open the app.

```
heroku open
```
