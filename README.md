# kea-centos-srpms
This repo contains srpm and spec for the ISC Kea DHCP server software. The repo owner is not affiliated with ISC.

## Build prerequisites and instructions

The following repositories and packages are needed to build the latest kea release on Centos 7.x

```yum install https://www.softwarecollections.org/en/scls/denisarnaud/boost157/epel-7-x86_64/download/denisarnaud-boost157-epel-7-x86_64.noarch.rpm```

```yum install epel-release autoconf automake libtool openssl-devel mariadb-devel postgresql-devel log4cplus-devel procps-ng python36 python3-rpm-macros boost157-devel```

## Setup build environment and build rpm

Follow this guide:
https://wiki.centos.org/HowTos/SetupRpmBuildEnvironment

or use mock:
https://github.com/rpm-software-management/mock/wiki

Install source rpm as normal user or as mock:

```rpm -i kea-<version>.el7.src.rpm
cd rpmbuild/SPECS
rpmbuild -ba kea.spec```
