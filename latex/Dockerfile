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

RUN axel http://download.opensuse.org/repositories/home:/jsundermeyer/xUbuntu_14.04/amd64/texstudio_2.10.8-5.1_amd64.deb

RUN apt-fast install -q -y  qt5-default qttools5-dev-tools libpoppler-qt5-1 libqt5script5 libqt5svg5

RUN dpkg -i texstudio_2.10.8-5.1_amd64.deb



CMD texstudio