FROM ubuntu:14.04
MAINTAINER Leandro Souza <leandrocsfrb@gmail.com>

ENV LANG en_US.UTF-8  
ENV LANGUAGE en_US:en  
ENV LC_ALL en_US.UTF-8 

RUN apt-get update 
RUN apt-get install -q -y wget
RUN wget --output-document gitbook-editor-5.0.4-linux-x64.deb http://downloads.editor.gitbook.com/download/linux-64-bit
RUN dpkg -i gitbook-editor-5.0.4-linux-x64.deb
RUN apt-get install -q -y libgtk2.0-0
RUN apt-get clean

CMD gitbook-editor