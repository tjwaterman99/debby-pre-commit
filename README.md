# debby-precommit

A pre-commit hook to run the [Debby dbt linter](https://www.debbyapp.com).

## Usage

Add a file named `.pre-commit-config.yaml` to the root of your repository (if you do not have one already).

Then add the following content.

```yaml
# .pre-commit-config.yaml
repos:
- repo: https://www.github.com/tjwaterman99/debby-pre-commit
  rev: v0.2.0
  hooks:
    - id: debby
```

Ensure pre-commit is installed on your system.

```
pip install pre-commit
```

Then install the hooks with

```
pre-commit install
```
