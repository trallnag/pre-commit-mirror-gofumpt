# Mirror of gofumpt for pre-commit

This repository mirrors [mvdan/gofumpt](https://github.com/mvdan/gofumpt)
releases and adds a pre-commit configuration so that people can use gofumpt
as a pre-commit hook. Note that the hook configuration uses golang as
language instead of script or system. This means that pre-commit handles
installing Go and gofumpt if they are not found.

To use the hook, add the following to your `.pre-commit-config.yaml` file:

```yaml
repo: https://github.com/trallnag/pre-commit-mirror-gofumpt
rev: v0.4.0
hooks:
  - id: gofumpt
```

How to update this repository once there is a new version of gofumpt?

1. Checkout both repos locally.
2. Delete everything in this repo except `README.md` and `.pre-commit-hooks.yaml`.
3. Copy over everything from gofumpt except `README.md` and `.github`.
4. Commit, tag, and push.

Maybe at some point pre-commit-mirror-maker will support Go. Until then this
workaround is good enough. There is an open issue for this [here](https://github.com/pre-commit/pre-commit-mirror-maker/issues/173).
