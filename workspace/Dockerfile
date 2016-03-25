FROM ubuntu:14.04
MAINTAINER leandrosouza <leandrocsfrb@gmail.com> 

RUN locale-gen en_US.UTF-8 

ENV LANG en_US.UTF-8  
ENV LANGUAGE en_US:en  
ENV LC_ALL en_US.UTF-8 



# Let the conatiner know that there is no tty
ENV DEBIAN_FRONTEND noninteractive

# Avoid ERROR: invoke-rc.d: policy-rc.d denied execution of start.
RUN echo "#!/bin/sh\nexit 0" > /usr/sbin/policy-rc.d

RUN apt-get update
RUN apt-get install -q -y libxtst6 libxrender1 libxi6



#COPY /home/leandro/Documentos/MATLAB_R2015b_glnxa64/full-iso-contents /tmp/MATLAB_R2015b_glnxa64



#/usr/local/MATLAB/R2015b/bin/matlab
#export LM_LICENSE_FILE=/home/leandro/Documentos/MATLAB_R2015b_glnxa64/crack/
#export LM_LICENSE_FILE=/home/leandro/Documentos/MATLAB_R2015b_glnxa64/crack/Matlab_R2015b_glnxa64.lic

#sh /home/leandro/Documentos/MATLAB_R2015b_glnxa64/full-iso-contents/install -inputFile /home/leandro/Documentos/installer_input.txt
#cp /home/leandro/Documentos/MATLAB_R2015b_glnxa64/crack/libcufft.so.7.0.28 /usr/local/MATLAB/R2015b/bin/glnxa64/libcufft.so.7.0.28
#cp /home/leandro/Documentos/MATLAB_R2015b_glnxa64/crack/libmwservices.so /usr/local/MATLAB/R2015b/bin/glnxa64/libmwservices.so


#cp /home/leandro/Documentos/MATLAB_R2015b_glnxa64/full-iso-contents /tmp/MATLAB_R2015b_glnxa64
