FROM harshjv/texlive-2015
MAINTAINER Leandro Souza <leandrocsfrb@gmail.com>

ENV LANG en_US.UTF-8  
ENV LANGUAGE en_US:en  
ENV LC_ALL en_US.UTF-8 

RUN apt-get update

RUN apt-get -f install -q -y axel libpoppler-qt4-4 libqt4-network libqt4-script libqt4-xml libqtcore4 libqtgui4 libqtwebkit4

RUN axel http://www.xm1math.net/texmaker/texmaker_ubuntu_14.04_4.5_amd64.deb

RUN dpkg -i texmaker_ubuntu_14.04_4.5_amd64.deb

ENV QT_GRAPHICSSYSTEM=native

CMD texmaker
