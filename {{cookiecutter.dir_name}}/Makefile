.PHONY: build
build:
	poetry build

.PHONY: format
format:
	poetry run black -v {{ cookiecutter.package_name }}
	poetry run black -v tests

.PHONY: install
install:
	poetry install

.PHONY: lint
lint:
	poetry run flake8 -v {{ cookiecutter.package_name }}
	poetry run flake8 -v tests

.PHONY: test
test:
	poetry run pytest -v
