# Version 0.0.1
FROM centos:6.6
MAINTAINER Evan Battle "evan.battle@emc.com"
ADD xmcli-3.0.1-11.tgz /tmp
WORKDIR /tmp
RUN yum -y update && yum -y install tar hostname git zsh sudo man python-crypto python-netaddr pytz && ./xmcli/install_xmcli.sh -install -silent
WORKDIR /

