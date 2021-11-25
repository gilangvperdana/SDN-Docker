FROM ubuntu:18.04

RUN apt update -y && \
    apt install python3 -y && \
    apt install unzip -y && \
    apt install wget -y && \
    apt install screen -y && \
    apt install sudo -y

RUN cd /home && \
    wget https://github.com/mininet/mininet/archive/refs/heads/master.zip && \
    unzip master.zip && rm master.zip && mv mininet-master mininet && \
    cd mininet/util/ && \ 
    ./install.sh -nfv

WORKDIR /home/mininet

EXPOSE 80
 