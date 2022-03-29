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

## Accessing Experimental Features
Experimental capability is required to be able to access experimental features. More information can be
referenced at [Cognite Authorization](https://docs.cognite.com/dev/guides/iam/authorization).

To access Geospatial experimental features, following capability is needed. Please contact your project administrator
regarding this.
```json
"capabilities": [ {
    "experimentAcl": {
        "actions": [ "USE"],
        "scope": {
            "experimentscope": {
                "experiments": [ "coregis" ]
            }
        }
    }
} ]
```
