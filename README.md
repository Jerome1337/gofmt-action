# Gofmt action

This action execute gofmt command and return the command output if fail.

## Inputs

### `gofmt-path`

Path used by gofmt command, default is `./`.

## Outputs

### `gofmt-output`

The gofmt output if the command fail.

## Example usage

```yaml
uses: Jerome1337/gofmt-action@v1.0.0
with:
  gofmt-path: './src'
````
