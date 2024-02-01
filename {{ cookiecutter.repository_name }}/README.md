[//]: # (todo: template)
# cookiecutter-terragrunt

A [`cookiecutter`](https://github.com/cookiecutter/cookiecutter) template for [`terragrunt`](https://github.com/gruntwork-io/terragrunt).

## dependencies

| name                                                               | description |
|--------------------------------------------------------------------|-------------|
| [terragrunt](https://github.com/gruntwork-io/terragrunt)           |             |
| [terraform](https://github.com/hashicorp/terraform)                |             |
| [terraform-docs](https://github.com/terraform-docs/terraform-docs) |             |
| [helm](https://github.com/helm/helm)                               |             |
| [helm-docs](https://github.com/norwoodj/helm-docs)                 |             |
| [pyenv](https://github.com/pyenv/pyenv)                            |             |
| [poetry](https://github.com/python-poetry)                         |             |

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
> `src/cookiecutter_terragrunt` is not currently used.

package:
```shell
poetry build
```

## usage

run:
```shell
cookiecutter https://github.com/generic-infrastructure/cookiecutter-terragrunt
```

test:
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
