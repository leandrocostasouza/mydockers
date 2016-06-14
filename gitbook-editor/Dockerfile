FROM ubuntu:16.04
MAINTAINER Leandro Souza <leandrocsfrb@gmail.com>

ENV LANG en_US.UTF-8  
ENV LANGUAGE en_US:en  
ENV LC_ALL en_US.UTF-8 

RUN apt-get update

RUN apt-get install -y curl wget

RUN curl -sL https://deb.nodesource.com/setup_4.x | -E bash -
RUN apt-get install -y nodejs
RUN npm install gitbook-cli -g
RUN mkdir temp
RUN cd tempBook
RUN gitbook init
RUN cd ..
RUN rm -r tempBook

#libs
RUN apt-get install -q -y libgtk2.0-0 libnotify4 libgconf-2-4 libnss3

RUN wget --output-document gitbook-editor-5.0.5-linux-x64.deb http://downloads.editor.gitbook.com/download/linux-64-bit

RUN dpkg -i gitbook-editor-5.0.5-linux-x64.deb

CMD gitbook-editor
