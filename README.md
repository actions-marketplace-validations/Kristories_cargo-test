# Cargo Test

Execute all unit and integration tests and build examples of a local package.

## Usage

See [action.yml](https://github.com/Kristories/cargo-test/blob/main/.github/workflows/main.yml) :

```yaml
on: [push]

jobs:
  test_job:
    runs-on: ubuntu-latest
    name: Testing
    steps:
      - uses: actions/checkout@v3
      - name: "Test local rust"
        uses: Kristories/cargo-test@v1.0.0
        with:
          manifest-path: './example-rust/Cargo.toml'
```

## License

The MIT License (MIT). Please see the [license file](LICENSE.md) for more information.