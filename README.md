# mkdocs mirror

Mirror of mkdocs package for pre-commit.

For pre-commit: see <https://github.com/pre-commit/pre-commit>

For mkdocs: see <https://github.com/mkdocs/mkdocs>

### Using mkcodc with pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
-   repo: https://github.com/Cube707/pre-commit-mirrors-mkdocs
    rev: '5bd6b1c'  # Use the sha / tag you want to point at
    hooks:
    -   id: mkdocs-build
```

### overriding `files`

note that [this repository] sets `files: (^mkdocs\.ya?ml$)|(^docs/)`, if you are configuring mkdocs
to use a different config-file and/or documentation folder, change the `files` key accordingly in your
`.pre-commit-config.yaml`.

[this repository]: https://github.com/Cube707/pre-commit-mirrors-mkdocs/blob/5bd6b1c919a0fde8a2c1e74741cd200c1b833a2f/.pre-commit-hooks.yaml#L9
