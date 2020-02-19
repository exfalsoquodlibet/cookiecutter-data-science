# Getting started

Create a Python 3 virtual environment, and install all packages in the `requirements.txt` file using the
following command:

```bash
make requirements
```
    
## `make` commands

The Makefile contains the central entry points for common tasks related to this project. The available rules for 
`make` are:

| Rule                 | Description                                 |
|----------------------|---------------------------------------------|
| `clean`              | Delete all compiled Python files            |
| `create_environment` | Set up Python interpreter environment       |
| `lint`               | Lint using `flake8`                         |
| `requirements`       | Install Python Dependencies                 |
| `test_environment`   | Test Python environment is set up correctly |
