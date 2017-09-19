## Create directories

```
mkdir jenkins-docker 
```

```
cd jenkins-docker
```

## Build

```
docker build -t jenkins-data -f Dockerfile-data .
```

```
docker build -t jenkins .
```

## Run

```
docker run --name=jenkins-data jenkins-data
```

```
docker run -p 8080:8080 -p 50000:50000 --name=jenkins-master --volumes-from=jenkins-data -d jenkins
```

```
docker exec jenkins-master cat /var/jenkins_home/secrets/initialAdminPassword
```
