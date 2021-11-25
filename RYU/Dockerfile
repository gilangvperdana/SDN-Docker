FROM ubuntu:18.04

RUN apt update -y && \
    apt-get install python3-ryu -y && \
    apt-get install git -y && \
    apt install screen -y && \
    apt install unzip -y \
    && apt-get clean

RUN cd /home && \
    wget https://github.com/faucetsdn/ryu/archive/refs/heads/master.zip && \
    unzip master.zip && rm master.zip && mv ryu-master ryu
    
WORKDIR /home/ryu/ryu/app

EXPOSE 6633
EXPOSE 8080