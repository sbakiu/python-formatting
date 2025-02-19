# python-formatting
Using:
* poetry
* pre-commit
* isort
* black
* flake8
* sqlfluff 
* pytest
* pytest-cov

for code formatting

Install dependencies:

```bash
poetry install
```

Run tests
```
poetry run pytest
```

Run tests with coverage report
```
poetry run pytest --cov-report term --cov=src tests/
```

Install pre-commit hooks
```bash
poetry run pre-commit install
```

Pre-commit check
```bash
poetry run pre-commit run --all-files
```

sqlfluff lints
```bash
poetry run sqlfluff lint dbt/dbt_test_project
```

## Versioning
```sh
VERSION=$(poetry version patch --short)
git commit -am "Bump Version"
git tag $VERSION
git push --tags
git push
```

Made with ❤️ by [datamax.ai](https://www.datamax.ai/).
