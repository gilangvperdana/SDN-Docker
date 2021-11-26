### OPENDAYLIGHT on Docker

```
Official : 
DockerHub : https://hub.docker.com/r/glefevre/opendaylight/
$ docker pull glefevre/opendaylight
$ docker run -d -p 6633:6633 -p 8181:8181 -p 8101:8101 --name=opendaylight glefevre/opendaylight

Self : 
DockerHub : https://hub.docker.com/r/gilangvperdana/sdn
$ docker pull gilangvperdana/sdn:odl 
$ docker run -d -p 6633:6633 -p 8181:8181 -p 8101:8101 --name=opendaylight gilangvperdana/sdn:odl

To inside the container : 
$ docker exec -it id_opendaylight_container bash

Install Some Features : 
$ ssh -p 8101 karaf@localhost 
Login with "karaf" for password

$ feature:install odl-restconf odl-l2switch-switch odl-mdsal-apidocs odl-dlux-all
$ feature:list --installed #To list all installed features
$ feature:list --installed #To list all ODL features
 
To acccess WEB Interface : 
$ ssh -p 8101 karaf@localhost 
Login with "karaf" for password

$ feature:install odl-dlux-all

Acess on ip_opendaylight:8181/apidoc/explorer/index.html 
OR
Access on ip_opendaylight:8181/index.html
Login with user : "admin" & password : "admin"

Acces on ip_opendaylight:6633 for OpenFlow
```
