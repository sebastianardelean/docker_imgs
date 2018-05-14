## Create directories

```
mkdir ocaml-docker
```

```
cd ocaml-docker
```

## Build

```
docker build -t ocaml-docker .
```


## Run



### Run interactively

```
docker run -ti ocaml-docker
```
### Run in batch mode

```
docker run -ti --mount type=bind,source="$(pwd)",target=/home/docker/scripts ocaml-docker 

```

```
docker run -ti --rm ocaml-docker
```


