# go-swagger2openapi
Example of converting swaggo generated swagger format files (2.0) to open api (3.0) for REST services written in Go.

## Converting local
```bash
docker run -p 8990:8080 swaggerapi/swagger-converter
```

*Use GitHub actions*

## View openapi
http://localhost:8080/swagger/doc.json

## View Swagger UI
http://localhost:8080/swagger/index.html