# kea-centos-srpms
This repo contains srpm and spec for the ISC Kea DHCP server software. The repo owner is not affiliated with ISC.

NOTICE: You need a newer version of boost-devel than what EPEL provides (1.53) in order to build kea-1.4.0-beta, because of the boost/asio/corutine.hpp dependency. I built it using the https://copr.fedorainfracloud.org/coprs/whosthere/boost/ repo. This will break anaconda dyninst, so I hope I will find a more proper workaround before the stable release.
