# OpenApi CodeGen

## Initial Setup
```
go mod init github.com/psychic-spoon/TestOpenAPI

go install github.com/deepmap/oapi-codegen/cmd/oapi-codegen@latest
```

Make sure the following works
```
oapi-codegen -version
```

## `Client`
```
oapi-codegen --package=main --generate types,client swagger.yaml > openapi.gen.go  
```

## `Server`
```
oapi-codegen --package=main  --generate types,server swagger.yaml > generatedserver.go 
```
