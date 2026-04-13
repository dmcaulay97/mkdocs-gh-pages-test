# integration-title

## Introduction

**UPDATE ME**  
This section should include a brief description of the integration and why it exists. For more information on creating valuable documentation, review the [SET documentation guidelines](https://github.ohio.edu/OIT/SET/blob/main/processes-and-guidelines/documentation-guidelines.md).  
**UPDATE ME**

## Development Notes

**UPDATE ME**  
This section should include any notes a developer should know about the integration which is not immediately apparent from the introduction or from the code itself. This may include (but is not limited to) notes regarding special setup for testing, additional documentation, or integration structure.  
**UPDATE ME**

## Config Maps and Secrets

**UPDATE ME**  
This section should include a list of config maps and secrets relevant to the integration.  
**UPDATE ME**

## Development Instructions

The CPU requests/limit and memory requests/limit have been set to small values. During development of an integration performance testing **MUST** be done to discover the values need to successfully run the integration.

The integration can be built and ran using command `skaffold dev`.

More information on Skaffold can be found [here](https://github.ohio.edu/OIT/SET/blob/main/development/development-with-skaffold.md).


## Python Type Hints

This template is configured to use Python type hints, which can be checked using MyPy static type checking. To check the type hints in your integration, run the following command in your terminal at your project root:

```Shell
mypy app
```

For additional information on Python typing and type checking, please see resources below:
- Python 3.11 Typing: https://docs.python.org/3.11/library/typing.html
- MyPy Type Checking: https://mypy.readthedocs.io/en/latest/getting_started.html
- MyPy Type Hint Cheat Sheet: https://mypy.readthedocs.io/en/latest/cheat_sheet_py3.html

## Python Linting and Formatting

This template includes a `ruff.toml` file intended to configure the [ruff](https://docs.astral.sh/ruff) tool. To run the ruff linter, run the following command in your terminal at your project root:

```Shell
ruff check app/
```

This will give you a list of all linter errors. You can run the previous command with the `--fix` flag to fix auto-fixable linted errors.

To see what the ruff formatter would change when reformatting, run the following command in your terminal at your project root:

```Shell
ruff format --check app/
```

This will give you a list of the files which would be reformatted. To do the reformat, run the following command:

```Shell
ruff format app/
```
