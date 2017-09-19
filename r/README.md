##Create directories

```
mkdir r-docker
```

```
cd r-docker
```

##Build

```
docker build -t r-docker .
```


##Run



###Run interactively

```
docker run -ti --rm r-scripts
```
###Run in batch mode

```
docker run -ti --name=r-scripts --mount type=bind,source="$(pwd)",target=/home/docker/scripts r-docker
```

```
docker run -ti --rm r-scripts /usr/bin/bash
```


