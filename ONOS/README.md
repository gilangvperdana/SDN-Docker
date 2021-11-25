### ONOS on Docker

```
DockerHub : https://hub.docker.com/r/onosproject/onos

Run command :
$ docker pull onosproject/onos
$ screen #optional
$ docker run -d -it -p 6640:6640 -p 6653:6653 -p 8101:8101 -p 8181:8181 -p 9876:9876 onosproject/onos

if you already use "screen" CTRL A+C to minimize and exit from container and POX will be run on background.

Test on ip_onos:6653 for forwarding data plane & ip_onos:8181/onos/ui/login.html
GUI WEB :
username : onos
password : rocks
```