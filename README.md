# Docker notes


<!-- vim-markdown-toc GFM -->

* [Using build args](#using-build-args)
* [Build and run](#build-and-run)

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