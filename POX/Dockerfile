FROM ubuntu:18.04

RUN apt update -y && \
    apt install python3 -y && \
    apt install unzip -y && \
    apt install wget -y && \
    apt install screen -y

RUN cd /home && \
    wget https://github.com/noxrepo/pox/archive/refs/heads/gar-experimental.zip && \
    unzip gar-experimental.zip && rm gar-experimental.zip && mv pox-gar-experimental pox

WORKDIR /home/pox

EXPOSE 6633
 