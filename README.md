# kea-centos-srpms
This repo contains srpm and spec for the ISC Kea DHCP server software. The repo owner is not affiliated with ISC.

NOTICE: You need a newer version of boost-devel than what EPEL provides (1.53) in order to build and install kea-1.4.0-beta, because of the boost/asio/corutine.hpp dependency. Use https://www.softwarecollections.org/en/scls/denisarnaud/boost157/ to avoid breaking packages depending on boost-devel 1.53.
