# `pre-commit` Hooks
`pre-commit` hooks to use with the `pre-commit` framework. This repository contains some custom hooks which are not available in the `pre-commit` repository.

## Setup
To use these hooks, you need to install the `pre-commit` framework. See [here](https://pre-commit.com/#install) for instructions. Then, add the hooks you want to use to your `.pre-commit-config.yaml` file. See [Adding pre-commit plugins to your project](https://pre-commit.com/#3-add-a-pre-commit-configuration) for instructions.

## Available hooks
### console.log detector
This hook detects `console.log` statements in your code. If it finds any, it will fail the commit.
```yaml
- repo: https://github.com/sameeramin/pre-commit-hooks.git
      rev: v1.0.1
      hooks:
          - id: check-console-log
```
