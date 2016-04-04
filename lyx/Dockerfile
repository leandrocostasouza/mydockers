FROM ubuntu:14.04
MAINTAINER leandrosouza <leandrocsfrb@gmail.com> 

RUN locale-gen en_US.UTF-8 

ENV LANG en_US.UTF-8  
ENV LANGUAGE en_US:en  
ENV LC_ALL en_US.UTF-8 

# Let the conatiner know that there is no tty
ENV DEBIAN_FRONTEND noninteractive

RUN apt-get install -q -y software-properties-common 

RUN add-apt-repository ppa:lyx-devel/release 
RUN apt-get update 
RUN apt-get install  -q -y lyx 

ENV  QT_X11_NO_MITSHM=1

# add abntex2
RUN apt-get install  -q -y wget xzdec

RUN tlmgr init-usertree
RUN tlmgr install abntex2
RUN tlmgr install babel-portuges


WORKDIR /root

RUN wget https://raw.githubusercontent.com/abntex/abntex2-contrib/master/lyx/abntex2-modelo-documento-filho.tex
RUN wget https://raw.githubusercontent.com/abntex/abntex2-contrib/master/lyx/abntex2-modelo-documento-filho.lyx
RUN wget https://raw.githubusercontent.com/abntex/abntex2-contrib/master/lyx/abntex2-modelo-trabalho-academico.tex
RUN wget https://raw.githubusercontent.com/abntex/abntex2-contrib/master/lyx/abntex2-modelo-trabalho-academico.lyx
RUN wget https://raw.githubusercontent.com/abntex/abntex2-contrib/master/lyx/2.1.X/abntex2.layout

RUN cp abntex2.layout /usr/share/lyx/layouts/abntex2.layout
RUN rm abntex2.layout

CMD lyx


