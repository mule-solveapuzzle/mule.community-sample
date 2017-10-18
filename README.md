# Mule Community & Docker example project

## What?

A sample Mule Community ESB project that runs in a docker image.

## How to Build?

```
mvn clean package docker:build
```

## How to run?

```
docker run -it -p "8081:8081" -p "1099:1099" community.test bash
>/opt/mule-standalone/bin/mule &
```

## How to test?

curl http://localhost:8888

## 
