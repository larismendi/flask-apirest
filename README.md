# flask-apirest

## Default params
### Go to config/default.py
SECRET_KEY = 'random key'

## Edit virtualenv activate file
export FLASK_APP="entrypoint:app"
export FLASK_ENV="development"
export APP_SETTINGS_MODULE="config.default"

## DB init
flask db init
flask db migrate -m "Initial_db"
flask db upgrade
## Run flask
flask run