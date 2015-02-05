# Version 0.0.1
FROM centos:latest
MAINTAINER Evan Battle "evan.battle@emc.com"
COPY NaviCLI-Linux-64-x86-en_US-7.33.3.0.72-1.x86_64.rpm /tmp/
WORKDIR /tmp
RUN yum -y update && yum -y install tar hostname git zsh sudo man && rpm -Uvh NaviCLI-Linux-64-x86-en_US-7.33.3.0.72-1.x86_64.rpm
WORKDIR /
ENV PATH $PATH:/opt/Navisphere/bin

