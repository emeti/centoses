# This is a CentOS image definiton with some packages added to make it an environment suitable for Linux Foundations training
# Added packages list (in brackets explanation of the command that needs a package)
# man, tree
# lvm2 (lvmcreate, used as an example in the training)
# glibc-langpack-en (to avoid errros shown for example by man, see issue https://github.com/CentOS/sig-cloud-instance-images/issues/154)
# FIXME /var/log/messages ... rsyslog ?
# nmcli (does not make too much sense in a docker container but is in NetworkManager and installed)
# killall mentioned in slides is not available
FROM centos:8
	RUN yum -y update \
	&& yum -y install passwd vim man tree lvm2 glibc-langpack-en file bash-completion NetworkManager nmap lsof

