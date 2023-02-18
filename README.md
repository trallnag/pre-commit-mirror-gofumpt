# Mirror of gofumpt for pre-commit

This repository mirrors [mvdan/gofumpt](https://github.com/mvdan/gofumpt)
releases and adds a pre-commit configuration so that people can use gofumpt
as a pre-commit hook.

To use the hook, add the following to your `.pre-commit-config.yaml` file:

```yaml
repo: https://github.com/trallnag/pre-commit-mirror-gofumpt
rev: v0.4.0
hooks:
  - id: gofumpt
```
