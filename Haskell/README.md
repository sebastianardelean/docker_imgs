## Create directories

```
mkdir stack-docker
```

```
cd stack-docker
```

## Build

```
docker build -t stack-docker .
```


## Run



### Run interactively

```
docker run -ti stack-docker
```
### Run in batch mode

```
docker run -ti --mount type=bind,source="$(pwd)",target=/home/docker/scripts stack-docker 

```

```
docker run -ti --rm stack-docker
```


