# openshift_poc
POC play with Openshift 4

## Deploy from JAR
We build the Docker Image from the JAR file, then deploy into Openshift Cluster

### Local Test
1. Under root path of this repo, build with following
```
docker build --build-arg JAR_FILE=build/libs/*.jar -t springio/gs-spring-boot-docker .
```
2. Run localhost for testing
```
docker run -p 8080:8080 -t springio/gs-spring-boot-docker
```
3. Check for errors. If no error, check service reachability, you should get 2XX/3XX
```
curl -vk localhost:8080
```

### Deployment
Coming soon...