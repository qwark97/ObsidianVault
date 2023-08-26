## mockery
The best option is to check [github page](https://github.com/vektra/mockery) of the project and download desired version from the "Releases" tab. Then, installation should be available within the $PATH

To use `mockery` inside the Go code, following annotation should be used (alongside with the parameters I consider as the most useful) above the interface declaration
```go
//go:generate mockery --name InterfaceName --case underscore --with-expecter --output ./mocks 
```
