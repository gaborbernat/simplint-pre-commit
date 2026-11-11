# simplint mirror

[![Mirror](https://github.com/gaborbernat/simplint-pre-commit/actions/workflows/main.yaml/badge.svg)](https://github.com/gaborbernat/simplint-pre-commit/actions/workflows/main.yaml)

Mirror of [simplint](https://github.com/gaborbernat/simplint) for
[pre-commit](https://github.com/pre-commit/pre-commit). The hook installs the prebuilt wheel from
[PyPI](https://pypi.org/project/simplint), so it needs no Rust toolchain and runs on
[pre-commit.ci](https://pre-commit.ci).

### Using simplint with pre-commit

Add it to your `.pre-commit-config.yaml`, between Ruff's check and format hooks:

```yaml
  - repo: https://github.com/gaborbernat/simplint-pre-commit
    rev: v0.10.3
    hooks:
      - id: simplint
```
