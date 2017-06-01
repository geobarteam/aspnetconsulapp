FROM microsoft/aspnetcore
WORKDIR /usr/local/bin
RUN apt-get update && \
    apt-get install -y \
    unzip \
    wget 


RUN wget https://releases.hashicorp.com/consul/0.8.3/consul_0.8.3_linux_amd64.zip && \
    unzip consul_0.8.3_linux_amd64.zip && \
    mkdir /consul && \
    mkdir /consul/data && \
    mkdir /consul/config

WORKDIR /app