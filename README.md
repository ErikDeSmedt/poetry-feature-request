# A poetry feature requests

This repo illustrates a feature request for `poetry`.
I want a way to install developer-dependencies of path dependencies.

## How to reproduce

```
poetry install
```

## Desired behavior

I expect typed `requests-types` is installed.

`./pyproject.toml` installs `awesome_lib` with the flag `developer=true`
`./awesome-lib/pyproject.toml` installs `requests-types` as a developer dependency.

## Observed behavior

`requests-types` is not installed
