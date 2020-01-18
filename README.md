# Travis lint pre-commit hook

This is a hook for [pre-commit] framework.

Check `.travis.yml` file for any issues with [`travis lint`][travis-lint]
command.

## Using travis lint with pre-commit

Add this to your `.pre-commit-config.yaml` file:

```yaml
  - repo: https://github.com/markosamuli/pre-commit-travis-lint
    rev: 'master' # Use the SHA / tag you want to point at
    hooks:
      - id: travis-lint
```

[pre-commit]: https://pre-commit.com/
[travis-lint]: https://github.com/travis-ci/travis.rb#lint
