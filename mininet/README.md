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

Run Topo mininet CLI (inside container) :
for ONOS :
$ mn --switch ovs,protocols=OpenFlow14 --controller remote,ip=IP:PORT --custom YOUR_TOPO.py --topo TOPONAME 

for POX :
$ mn --custom YOUR_TOPO.py --topo TOPONAME --controller=remote,ip=IP:PORT

for RYU :
$ mn --custom YOUR_TOPO.py --topo TOPONAME --controller=remote,ip=IP:PORT
```
