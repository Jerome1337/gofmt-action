# Gofmt Action

This action execute gofmt command and return the command output if fail.

## Inputs

`gofmt-path`

Path where your Go files are.
This path will be used by gofmt command to check files formatting.

Default one is the repository root (`./`).

## Outputs

`gofmt-output`

The gofmt output if the command fail.

For Example:

```bash
All the following files are not correctly formatted
handlers/writer.go
services/writerServices.go
```

## Example Usage

```yaml
uses: Jerome1337/gofmt-action@v1.0.2
with:
  gofmt-path: './src'
````
