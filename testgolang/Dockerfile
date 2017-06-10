FROM ubuntu:14.04

RUN apt-get update -y && apt-get install --no-install-recommends -y -q \
    openssh-client \
    curl \
    build-essential \
    bison \
    ca-certificates \
    wget \
    vim-gnome \
    firefox \
    graphviz


RUN wget https://storage.googleapis.com/golang/go1.6.2.linux-amd64.tar.gz

RUN sudo tar -C /usr/local -xzf go1.6.2.linux-amd64.tar.gz

ENV GOROOT=/usr/local/go
ENV PATH=$GOROOT/bin:$PATH

# To remove older version of go
# sudo rm -rf /usr/local/go
