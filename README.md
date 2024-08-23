# Protos
All proto files for Aristogram gRPC services.

### How to use

Add module to your application using the following command:
```shell
go mod github.com/aristogram/protos
```

### Code generate

If you want to change some protofiles, then you should generate new golang files using the following command:
```shell
protoc -I proto proto/*/*.proto --go_out=./gen/go/ --go_opt=paths=source_relative --go-grpc_out=./gen/go/ --go-grpc_opt=paths=source_relative
```