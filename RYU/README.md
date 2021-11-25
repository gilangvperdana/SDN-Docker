### RYU on Docker

```
DockerHub : https://hub.docker.com/repository/docker/gilangvperdana/sdn
$ docker pull gilangvperdana/sdn:ryu

Build from Scratch :
$ docker build -t ryu .
$ docker run -it -d -p 6633:6633 -p 8080:8080 ryu

Run command :
$ docker exec -it id_ryu_container bash
$ screen #optional
$ ryu-manager simple_switch_stp_13.py gui_topology/gui_topology.py

if you already use "screen" CTRL A+C to minimize and exit from container and POX will be run on background.

Test on ip_ryu:6633 for forwarding data plane port & ip_ryu:8080 for GUI.
```