# Version 0.0.1
FROM centos:latest
#FROM seancummins/cummis
MAINTAINER Sean Cummins "sean.cummins@emc.com"
ADD se7400-Linux-i386-ni.tar.gz /tmp
WORKDIR /tmp
RUN yum -y update && yum -y install tar hostname glibc.i686 git zsh sudo man && ./se7400_install.sh -install -64bit -silent
WORKDIR /
ENV PATH $PATH:/opt/emc/SYMCLI/bin
ENV SYMCLI_OFFLINE 1
