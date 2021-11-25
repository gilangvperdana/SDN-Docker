### MININET on Docker

```
DockerHub : https://hub.docker.com/repository/docker/gilangvperdana/sdn
$ docker pull gilangvperdana/sdn:mininet

Run command :
$ docker run -d -it -p 81:80 gilangvperdana/sdn:mininet

Move your py topo to inside Mininet Container :
$ docker cp ./your_file id_mininet_container:/home/mininet/
```