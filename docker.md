# Docker useful cli

* show all container
```Shell
docker ps -a
```
* list images
```Shell
docker image ls 
```
* start container
```Shell
docker run -it <image>
```
```-it``` instructs Docker to allocate a pseudo-TTY connected to the container’s stdin<br />
"--rm"		Automatically remove the container when it exits<br />
"-w /path/to/dir/" set working directory<br />
"-v /path/local:/path/container" mount host dir to container dir<br />
"-p 80(host port):80(container port)" bounding ports<br />
"--name name" gives name to container<br />
"--gpus all" enable gpu for container<br />

* get to bash of container
```Shell
docker exec -ti <container> bash

docker exec -ti <container> <commend>
```
use container's id or name

* commit change of container to image
```Shell
docker commit <containerId> <newImageId>
```

* stop and remove container
```Shell
docker stop <containerId>
docker rm <containerId>
```

* image backup
```Shell
docker save <image> > <image>.tar

docker load  < <image>.tar
```

