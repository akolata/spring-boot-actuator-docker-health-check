# Config Service

## Maven

### Build .jar
```shell
mvn -DskipTests clean package
```

## Docker

### Build image
```shell
docker build . \
  --tag spring-boot-healthcheck-demo/config-service:latest
```

### Run image
```shell
docker run \
  -d \
  --rm \
  --name=spring-boot-healthcheck-demo-config-service \
  -p 8888:8888 \
  spring-boot-healthcheck-demo/config-service:latest
```