# Contributing

Thank you for helping. This repository is the organization-level configuration for the
[cubic](https://cubic.dev) AI code reviewer: one `cubic.yaml` that applies to every repository
in the organization without a `cubic.yaml` of its own. There is no code, no build and no test
suite, so a change here is a change to how every one of those repositories is reviewed.

## Principles

- **One shared file.** Change the shared settings here rather than adding a `cubic.yaml` to a
  single repository: a repository-level file replaces these fields for that repository.
- **Ignore only what cannot be reviewed usefully.** An ignore pattern is for generated or
  vendored files with their own check against their source, and for lockfiles. Never ignore
  source code to quiet a reviewer.
- **Say why in the file.** When you add or change an ignore pattern or a setting whose reason
  is not plain from its name, put a comment next to it saying what it covers and why. A pull
  request description is not enough on its own, because the file outlives it.

## Checking a change

- Keep the file valid against the schema named on its first line,
  <https://cubic.dev/schema/cubic-repository-config.schema.json> (documented at
  <https://docs.cubic.dev/configure/cubic-yaml>). An editor with the YAML language server
  checks it as you type.
- Use only synthetic examples in pull request text: `example-repo`, `/path/to/...`. Never
  include real hosts, account ids, tokens or names.
- Security issues go through private vulnerability reporting (see `SECURITY.md`), not public
  issues.

By contributing, you agree that your contributions are licensed under the Apache License 2.0.

## Code of conduct

This project follows the [Contributor Covenant](CODE_OF_CONDUCT.md).
