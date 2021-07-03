This action sets git user as `github-actions[bot]`.

```sh
git config user.email "41898282+github-actions[bot]@users.noreply.github.com"
git config user.name "github-actions[bot]"
```

This allows committing changes inside a workflow run.

## Usage

```yaml
steps:
  - uses: actions/checkout@v2
  - uses: git-actions/set-user@v1
  - run: |
      # Make changes
      git commit -am 'Add changes'
      git push
```

## License

[MIT](LICENSE)
