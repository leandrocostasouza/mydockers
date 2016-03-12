FROM leandrosouza/latex

RUN axel http://download.opensuse.org/repositories/home:/jsundermeyer/xUbuntu_14.04/amd64/texstudio_2.10.8-5.1_amd64.deb

RUN apt-fast install -q -y  qt5-default qttools5-dev-tools libpoppler-qt5-1 libqt5script5 libqt5svg5

RUN dpkg -i texstudio_2.10.8-5.1_amd64.deb

RUN apt-fast clean

CMD texstudio
