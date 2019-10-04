# Circulate - Demo App for AwesomeCI

This is a working application that you can use.

It's a 'social blogging' web application similar to Twitter. Users can create accounts, make posts, follow users and comment on posts. You can *circualate* your thoughts and ideas :-)

**Original Author Credit:** This is directly based on Miguel Grinberg's excellent [Flasky](https://github.com/miguelgrinberg/flasky) application.

The application uses Python and Flask for the backend.

**IMPORTANT:**

- You will not need to install or setup a Python environment to follow the tutorial - you can follow along by making edits to config on GitHub if you wish.

## Running locally

- Install PostgreSQL (tested with 9.6.5)
- Install Python (tested with Python 3.6.2)
- Fork or clone this repository
- Create and activate a virtual environment
- Enter the following commands:

```
createdb circulate
pip install -r requirements/dev.txt
python manage.py deploy
python manage.py runserver
```

You can now test the app locally with the Flask development server.

## Tests

The app runs various tests:

- unit tests for database models (using unittest)
- unit tests for client view functions (using Flask Test Client)
- unit tests for the API (using Flask Test Client)
- integration tests for logging in etc (using Selenium and ChromeDriver)

It uses [unittest-xml-reporting](https://github.com/xmlrunner/unittest-xml-reporting) for JUNIT style report generation.

See the `tests` directory for details.

`python manage.py test` to run the tests locally.


## TODO

- add parallelization
- test with multiple python versions
- run with coverage
- make email testing work on with mailhog
- make email work on the deployed Heroku app

---
