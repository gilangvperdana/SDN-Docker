### MININET on Docker

```
DockerHub : https://hub.docker.com/repository/docker/gilangvperdana/sdn
$ docker pull gilangvperdana/sdn:mininet

Run command :
$ docker run -it --rm --privileged -e DISPLAY \
             -v /lib/modules:/lib/modules \
             gilangvperdana/sdn:mininet

Move your py topo to inside Mininet Container :
$ docker cp ./your_file id_mininet_container:/root/
```