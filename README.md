# Geospatial Examples

## Install
Poetry: python packaging and dependency management

```commandline
curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
```

Install dependencies
```bash
poetry install
```
## Setup Authentication
Update following environment variables
```bash
export OAUTH_TOKEN_URL=...
export OAUTH_CLIENT_ID=...
export OAUTH_CLIENT_SECRET=...
export OAUTH_TOKEN_SCOPES=...
export COGNITE_API_PROJECT=...
export COGNITE_CLIENT_NAME=...
```
## Run notebooks
```bash
poetry run jupyter notebook
```
