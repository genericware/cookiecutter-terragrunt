# cookiecutter-terragrunt

A [`cookiecutter`](https://github.com/cookiecutter/cookiecutter) template for [`terragrunt`](https://github.com/gruntwork-io/terragrunt) projects.

## dependencies

| name                                       | description                                |
|--------------------------------------------|--------------------------------------------|
| [pyenv](https://github.com/pyenv/pyenv)    | python version management                  |
| [poetry](https://github.com/python-poetry) | python packaging and dependency management |

## install

development:
```shell
poetry install
poetry shell
pre-commit install
```

production:
```shell
poetry install --without dev
```

## build

> [!IMPORTANT]
> `src/cookiecutter-terragrunt` is not currently used.

package:
```shell
poetry build
```

## run

template:
```shell
cookiecutter https://github.com/generic-infrastructure/cookiecutter-terragrunt
```

test:
```shell
pytest .
```

coverage:
```shell
coverage run -m pytest && coverage report -m
```

matrix:
```shell
tox run
```

doc:
```shell
make -C docs html
```

check:
```shell
pre-commit run
```

format:
```shell
black .
```

lint:
```shell
ruff .
```

type:
```shell
mypy .
```
