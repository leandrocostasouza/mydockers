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

ENV QT_X11_NO_MITSHM=1

CMD lyx 
