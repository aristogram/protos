# Protos
All proto files for Aristogram gRPC services.

### Code generate

If you want to change some protofiles, then you should generate new golang files using the following command: 

```protoc -I proto proto/sso/*.proto --go_out=./gen/go/ --go_opt=paths=source_relative --go-grpc_out=./gen/go/ --go-grpc_opt=paths=source_relative```