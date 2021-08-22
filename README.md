# go-swagger2openapi
Example of converting swaggo generated swagger format files (2.0) to open api (3.0) for REST services written in Go.

## Generate documentation

### Generate local documentation
```bash
swag init
docker run --name converter --rm -p 8990:8080 swaggerapi/swagger-converter
docker run -v $(pwd):/api --link converter -it --rm -w /api curlimages/curl:latest sh convert-localhost-v2v3.sh
```

*Use GitHub actions*

## Execute project
```bash
go run .
```

## View openapi
http://localhost:8080/swagger/doc.json

## View Swagger UI
http://localhost:8080/swagger/index.html