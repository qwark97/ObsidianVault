### Running tests with coverage
```bash
go test ./... -cover -coverprofile=c.out -coverpkg=./...
```
### Generating html coverage output
```bash
go tool cover -html=filtered.out -o coverage.html
```
