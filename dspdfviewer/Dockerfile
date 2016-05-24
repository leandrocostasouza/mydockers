FROM ubuntu:16.04
MAINTAINER Leandro Souza <leandrocsfrb@gmail.com>

RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -q -y software-properties-common 

RUN add-apt-repository ppa:dannyedel/dspdfviewer
RUN apt-get update && apt-get install -q -y dspdfviewer
RUN dspdfviewer
