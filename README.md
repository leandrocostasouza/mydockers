![](http://kodi.tv/wp-content/themes/paradise/Paradise/images/logo.png) 

Docker-Kodi 
=====================

[![Stories in Ready](https://badge.waffle.io/leandrocostasouza/docker-kodi.png?label=ready&title=Ready)](https://waffle.io/leandrocostasouza/docker-kodi) [![Stories in Progress](https://badge.waffle.io/leandrocostasouza/docker-kodi.png?label=In%20Progress&title=In%20Progress)](https://waffle.io/leandrocostasouza/docker-kodi) [![Build Status](https://travis-ci.org/leandrocostasouza/docker-kodi.svg?branch=master)](https://travis-ci.org/leandrocostasouza/docker-kodi) 

Kodi ppa:team-xbmc docker

docker run -it --user=$USER --env="DISPLAY" --workdir="/home/$USER" --volume="/home/$USER:/home/$USER" --volume="/etc/group:/etc/group:ro" --volume="/etc/passwd:/etc/passwd:ro" --volume="/etc/shadow:/etc/shadow:ro" --volume="/etc/sudoers.d:/etc/sudoers.d:ro" --volume="/tmp/.X11-unix:/tmp/.X11-unix:rw" leandrosouza/docker-kodi


To view in Windows use [MobaXterm](http://mobaxterm.mobatek.net/)
