dnscrypt-proxy-openwrt
======================


You find this package in the new OpenWrt feed : [net/dnscrypt-proxy](https://github.com/openwrt/packages/tree/master/net/dnscrypt-proxy)

##Deprecated

[dnscrypt](https://github.com/opendns/dnscrypt-proxy) OpenWrt Makefile for package building, based on [Black Roland](https://github.com/black-roland/exOpenWrt) one (thank you :smile: )

Depends on [libsodium](https://github.com/jedisct1/libsodium). OpenWrt package and Makefile available at https://github.com/damianorenfer/libsodium-openwrt

###Build for your platform

1. Install the OpenWrt environnement : http://wiki.openwrt.org/doc/howto/buildroot.exigence
2. Use the Makefile of this repo to build your dnscrypt-proxy package. Example : http://wiki.openwrt.org/doc/devel/packages
3. From the buildroot dir : `make package/dnscrypt-proxy/{clean,prepare,configure,compile} V=s`

###Installation

1. Install [libsodium package](https://github.com/damianorenfer/libsodium-openwrt)
2. Upload the dnscrypt-proxy_1.4.0-1_{PLATFORM}.ipk to your OpenWrt router : `scp dnscrypt-proxy_1.4.0-1_{PLATFORM}.ipk root@ip_of_your_openwrt:~`
3. Now remote login to your OpenWrt : `ssh root@ip_of_your_openwrt`
4. Remote install the package : `opkg install dnscrypt-proxy_1.4.0-1_{PLATFORM}.ipk`
5. Follow configuration instructions : http://wiki.openwrt.org/inbox/dnscrypt#configuration
