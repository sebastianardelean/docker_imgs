## Create directories

```
mkdir clash-docker
```

```
cd clash-docker
```

## Build

```
docker build -t clash-docker .
```


## Run



### Run interactively

```
docker run -ti clash-docker
```
### Run in batch mode

```
docker run -ti --mount type=bind,source="$(pwd)",target=/home/docker/scripts clash-docker 

```

```
docker run -ti --rm clash-docker
```


Or, using background container

```
docker run -d --name devtest -it --mount type=bind,source="$(pwd)",target=/home/docker/scripts clash-docker 
```

And use 

```
docker container exec name_container command