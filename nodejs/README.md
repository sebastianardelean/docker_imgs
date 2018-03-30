## Create directories

```
mkdir node-docker
```

```
cd node-docker
```

## Build

```
docker build -t node-docker .
```


## Run



### Run interactively

```
docker run -ti node-docker
```
### Run in batch mode

```
C=$(docker run -i -d node-docker sh)
docker exec -it $C sh

```


