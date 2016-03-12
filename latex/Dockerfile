FROM ubuntu:14.04
MAINTAINER Leandro Souza <leandrocsfrb@gmail.com>

ENV LANG en_US.UTF-8  
ENV LANGUAGE en_US:en  
ENV LC_ALL en_US.UTF-8 

RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -q -y software-properties-common 
RUN add-apt-repository ppa:saiarcot895/myppa -y 
RUN apt-get update 
RUN apt-get install -q -y axel apt-fast
RUN apt-fast install -q -y texlive-full
RUN apt-get clean
RUN apt-fast clean
