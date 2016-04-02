FROM alpine:3.3
MAINTAINER leandrosouza <leandrocsfrb@gmail.com> 
RUN echo "http://nl.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories 
RUN apk update
RUN apk add alpine-desktop xfce4 thunar-volman faenza-icon-theme
ENTRYPOINT [ "startxfce4" ]
