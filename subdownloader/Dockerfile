FROM ubuntu:14.04
MAINTAINER Leandro Souza <leandrocsfrb@gmail.com>

ENV LANG en_US.UTF-8  
ENV LANGUAGE en_US:en  
ENV LC_ALL en_US.UTF-8 

RUN apt-get update 
RUN apt-get install -q -y axel
RUN axel http://launchpadlibrarian.net/188331215/subdownloader_2.0.18-1_all.deb
RUN apt-get -f install -q -y  python-qt4 python-crypto python-kaa-metadata
RUN apt-get clean
RUN dpkg -i subdownloader_2.0.18-1_all.deb

ENV QT_GRAPHICSSYSTEM=native

CMD subdownloader
