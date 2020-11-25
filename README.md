# Gofmt Action

This action execute gofmt command and return the command output if fail.

## Inputs

`gofmt-path`

Path where your Go files are.
This path will be used by gofmt command to check files formatting.

Default one is the repository root (`./`).

`gofmt-flags`

Custom flags to pass to gofmt. 
See [gofmt docs](https://golang.org/cmd/gofmt/) for available flags.

Default behaviour is to list all file paths with incorrect formatting (`-l`).

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
uses: Jerome1337/gofmt-action@v1.0.4
with:
  gofmt-path: './src'
  gofmt-flags: '-l -d'
````
