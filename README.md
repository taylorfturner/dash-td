# dash-td
 [![Build Status](https://travis-ci.org/taylorfturner/dash-td.svg?branch=master)](https://travis-ci.org/taylorfturner/dash-td) [![Updates](https://pyup.io/repos/github/taylorfturner/dash-td/shield.svg)](https://pyup.io/repos/github/taylorfturner/dash-td/) [![Python 3](https://pyup.io/repos/github/taylorfturner/dash-td/python-3-shield.svg)](https://pyup.io/repos/github/taylorfturner/dash-td/) [![Coverage](https://codecov.io/github/taylorfturner/dash-td/coverage.svg?branch=master)](https://codecov.io/github/taylorfturner/dash-td?branch=master) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)


Dash dashboard for managing important metrics for portfolio and accounts in TD Ameritrade


## Usage
If you are on Linux and you have [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/) installed you can run the script `utility/setup_virtualenv_and_repo.sh` to:

- create a python virtual environment and activate it
- install all project dependencies from `requirements.txt`
- create a git repository
- create your `Initial commit`

Here is how you run the script:

```shell
cd dash-td
# mind the dot!
. utility/setup_virtualenv_and_repo.sh
```

Then you will need to create an `.env` file where to store your environment variables (SECRET key, plotly credentials, API keys, etc). Do NOT TRACK this `.env` file. See `.env.example`.

Run all tests with a simple:

```
pytest -v
```


## Run your Dash app
Check that the virtual environment is activated, then run:

```shell
cd dash_td
python app.py
```

## Code formatting
To format all python files, run:

```shell
black .
```

## Pin your dependencies

```shell
pip freeze > requirements.txt
```

## Deploy on Heroku
Follow the [Dash deployment guide](https://dash.plot.ly/deployment) or have a look at the [dash-heroku-template](https://github.com/plotly/dash-heroku-template)
