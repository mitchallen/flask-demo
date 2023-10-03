flask-demo
==

## Usage

* Start Docker
* Run this in VS Code as part of a Dev container

```sh
flask run
```

## Freezing

### Save installation

```sh
python -m pip freeze > requirements.txt
```

Install (handled in dev container config):

```sh
python -m pip install -r requirements.txt
```

Via dev container (.devcontainer/devcontainer.json):

pip and pip3 are mapped to the same thing:

```json
// Use 'postCreateCommand' to run commands after the container is created.
"postCreateCommand": "pip3 install --user -r requirements.txt"
```

## References

* [Flask Installation](https://flask.palletsprojects.com/en/3.0.x/installation/)
* [Flask: A Minimal Application](https://flask.palletsprojects.com/en/3.0.x/quickstart/#a-minimal-application)
* [Deploying to Production](https://flask.palletsprojects.com/en/3.0.x/deploying/)
* [Setting up Flask applications on PythonAnywhere](https://help.pythonanywhere.com/pages/Flask/)
* [Deploy Python Service to Google Cloud Run](https://cloud.google.com/run/docs/quickstarts/build-and-deploy/deploy-python-service)
