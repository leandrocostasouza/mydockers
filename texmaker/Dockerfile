FROM leandrosouza/latex

RUN apt-get -f install -q -y libpoppler-qt4-4 libqt4-network libqt4-script libqt4-xml libqtcore4 libqtgui4 libqtwebkit4

RUN axel http://www.xm1math.net/texmaker/texmaker_ubuntu_14.04_4.5_amd64.deb

RUN dpkg -i texmaker_ubuntu_14.04_4.5_amd64.deb

CMD texmaker
