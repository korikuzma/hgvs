# Dev Containers

Instructions for working with hgvs using Dev Containers

## Setup Installation

Inside command pallete: (this will take a few moments)

```
Dev Containers: Rebuild and Reopen in Container
```

You should see `Dev Container: biocommons @ desktop-linux` on the bottom left hand corner of VS Code.

Install depdendencies:

```shell
pip install --upgrade setuptools
pip install -e .[dev]
```

To run tests:

```shell
make test
```
