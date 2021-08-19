# git-sparse-checkout-buildkite-plugin

Buildkite plugin that performs a bare-bones partial clone of a repo and then a sparse-checkout of specified directories

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
  - command: echo git-sparse-checkout
    plugins:
      - highspot/git-sparse-checkout#v0.0.1:
          paths: 
            - "dir1"
            - "dir2"
```

## Configuration

### `paths` (Required, list)

List of directory paths to sparse checkout.

## Developing

To run the tests:

```shell
docker-compose run --rm tests
```

## Contributing

1. Fork the repo
2. Make the changes
3. Run the tests
4. Commit and push your changes
5. Send a pull request
