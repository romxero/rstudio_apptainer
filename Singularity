Bootstrap: docker
From: rockylinux:8

%post

sed -i 's/enabled\=0/enabled\=1/g' /etc/yum.repos.d/Rocky-PowerTools.repo
sed -i 's/enabled\=0/enabled\=1/g' /etc/yum.repos.d/Rocky-Plus.repo

#
dnf -y install epel-release 
export R_VERSION=4.4.0
#
#
dnf -y install https://cdn.rstudio.com/r/centos-8/pkgs/R-${R_VERSION}-1-1.x86_64.rpm
# we need a version of R installed for this to work./ 
dnf -y install https://download2.rstudio.org/server/rhel8/x86_64/rstudio-server-rhel-2024.04.2-764-x86_64.rpm



%environment
export LC_ALL=C.UTF-8


%runscript
/dev/null








