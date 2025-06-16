# Hellsehen

Clairvoyance fork with better UX.

[![Original README](https://github.com/nikitastupin/clairvoyance/)

## Dev env setup

```bash
pyenv install 3.12.3
pyenv local 3.12.3
poetry env use $(pyenv which python)
poetry lock
potry install
```

## Test

```bash
poetry run pytest
```

## Run

```bash
pyenv local 3.12.3
poetry env use $(pyenv which python)
poetry run python -m clairvoyance https://example.com/graphql -o schema.new.gql -w target.wl -wv -c 10 -i schema.gql -v -H ./headers.txt
```

# What's new

* --headers argument now accepts file
* exit on 403 error
* strict python version
