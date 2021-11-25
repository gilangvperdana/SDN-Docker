### POX on Docker

```
DockerHub : https://hub.docker.com/repository/docker/gilangvperdana/sdn
$ docker pull gilangvperdana/sdn:pox

Build from Scratch :
$ docker build -t pox .
$ docker run -it -d -p 6633:6633 pox

Run command :
$ docker exec -it id_pox_container bash
$ screen #optional
$ ./pox.py samples.pretty_log forwarding.l2_pairs openflow.discovery --eat-early-packets openflow.spanning_tree --no-flood --hold-down

if you already use "screen" CTRL A+C to minimize and exit from container and POX will be run on background.

Test on ip_pox:6633
```