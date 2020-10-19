# Docker notes


<!-- vim-markdown-toc GFM -->

* [Using build args](#using-build-args)
* [Build and run](#build-and-run)
* [Run with mounted local dir](#run-with-mounted-local-dir)
* [Usage](#usage)

<!-- vim-markdown-toc -->

## Using build args
```
docker build . --tag foo --build-arg BASE=5.8
```

## Build and run
```
<snip>
Successfully built e56719b352cf
Successfully tagged foo:latest...
```

```
docker run -it e56719b352cf /bin/bash
```

## Run with mounted local dir
```
docker run -it --volume $PWD:/home/project e56719b352cf /bin/bash
```

## Usage
Real time scoreboard of memory usage:
```
docker stats
```
