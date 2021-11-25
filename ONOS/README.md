### ONOS on Docker

```
OFFICIAL :
DockerHub : https://hub.docker.com/r/onosproject/onos
$ docker pull onosproject/onos

SELF : 
DockerHub : https://hub.docker.com/repository/docker/gilangvperdana/sdn
$ docker pull gilangvperdana/sdn:onos

Run command :
$ screen #optional
$ docker run -d -it -p 6640:6640 -p 6653:6653 -p 8101:8101 -p 8181:8181 -p 9876:9876 onosproject/onos

Test on ip_onos:6653 for forwarding data plane & ip_onos:8181/onos/ui/login.html
GUI WEB :
username : onos
password : rocks
```