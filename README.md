# Mule Community & Docker example project

## What?

A sample Mule Community ESB project that runs in a docker image.

## How to Build?

```
mvn clean package docker:build
```

## How to run?

```
docker run -d -p 8081:8081 -p 1099:1099 community.test
```

## How to test?
```
curl http://localhost:8081/countries
```

Returns a list of countries

## Push to docker hub

```
docker login
docker tag community.test:latest npiper/community.test:latest
docker push
```

# References

Cloudfoundry java logging	- Env Var VCAP_APPLICATION value used
https://github.com/pivotalservices/cloudfoundry-java-logging

