# python-cli-template

cookiecutter --no-input gh:kuzxnia/python-cli-template program_name=<project_name_here>


# features

* Docker

* pytest - test
* pytest-cov

* black
* mypy
* isort
* flake8
* pylint
* bandit
* pre-commit

* pyproject.toml
* pipfile
* Makefile

'''bash
# Install pipx if pipenv and cookiecutter are not installed
python3 -m pip install pipx
python3 -m pipx ensurepath

# Install pipenv using pipx
pipx install pipenv

# Use cookiecutter to create project from this template
pipx run cookiecutter gh:sourcery-ai/python-best-practices-cookiecutter

# Enter project directory
cd <repo_name>

# Initialise git repo
git init

# Install dependencies
pipenv install --dev

# Setup pre-commit and pre-push hooks
pipenv run pre-commit install -t pre-commit
pipenv run pre-commit install -t pre-push
'''
