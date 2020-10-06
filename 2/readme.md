# How-to:
Must be run on an azure virtual machine or can be built locally with docker that will `go test`
## Test and build
A docker image will be built if all the go tests pass.
```
docker build -t kpmg2 .
```
### You can also run natively with go
With specific key
```
go get -d
go run ./main.go -key compute.name
```
or
```
go get -d
go run ./main.go -key network.interface.0.ipv4.ipAddress.0.privateIpAddress
```
