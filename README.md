# Onos Docker Installer

Publishing the project on the docker
```
  $ docker-compose up
```

Terminate a project live on Docker
```
  $ docker-compose down
```

Controller user information
```
  host: http://localhost:8181/onos/ui
  user(id): onos
  password: rocks
```
#### In order to select the subnet of the Onos project, a new bridge should be added to the docker network.
```
docker network create \
  --driver=bridge \
  --subnet=172.28.0.0/16 \
  --ip-range=172.28.5.0/24 \
  --gateway=172.28.5.254 \
  br0
```
