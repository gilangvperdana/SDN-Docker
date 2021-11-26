### OPENDAYLIGHT on Docker

```
DockerHub : https://hub.docker.com/r/glefevre/opendaylight/
$ docker pull glefevre/opendaylight

Run command :
$ docker exec -it id_opendaylight_container bash
$ docker run -d -p 6633:6633 -p 8181:8181 -p 8101:8101 --name=opendaylight glefevre/opendaylight

To acccess WEB Interface : 
$ ssh -p 8101 karaf@localhost 
Login with "karaf" for password

$ feature:install odl-dlux-all
Access on ip_opendaylight:8181/index.html
Login with user : "admin" & password : "admin"
Acces on ip_opendaylight:6633 for OpenFlow
```