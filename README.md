shadowsocks-openwrt
===================

A package of shadowsocks for OpenWrt

## background
This is a package description for OpenWrt's buildroot, which grabs source from github.com/haohaolee.com/shadowsocks-libev.


## build from source
Download OpenWrt source from [dev][] or SDK from [downloads][]. And go to the root of the SDK or source. e.g.:

    [haohaolee@arch OpenWrt-SDK]$ ls -l
    total 76
    -rw-r--r-- 1 haohaolee users    32 Aug 16  2011 Config.in
    drwxr-xr-x 2 haohaolee users  4096 Dec 30 03:16 dl
    drwxr-xr-x 2 haohaolee users  4096 Nov 26 11:41 docs
    -rw-r--r-- 1 haohaolee users   567 Nov 26 19:03 feeds.conf.default
    drwxr-xr-x 3 haohaolee users  4096 Nov 26 19:03 include
    -rw-r--r-- 1 haohaolee users 17992 Aug 16  2011 LICENSE
    -rw-r--r-- 1 haohaolee users  1161 Aug 16  2011 Makefile
    drwxr-xr-x 4 haohaolee users  4096 Dec 28 18:12 package
    -rw-r--r-- 1 haohaolee users   337 Aug 16  2011 README.SDK
    -rw-r--r-- 1 haohaolee users  9563 Nov 26 11:41 rules.mk
    drwxr-xr-x 4 haohaolee users  4096 Nov 26 11:41 scripts
    drwxr-xr-x 5 haohaolee users  4096 Nov 26 19:03 staging_dir
    drwxr-xr-x 3 haohaolee users  4096 Nov 26 19:03 target
    
    [haohaolee@arch OpenWrt-SDK]$ git clone https://github.com/haohaolee/shadowsocks-openwrt.git package/shadowsocks-openwrt
    ...
    ...
    [haohaolee@arch OpenWrt-SDK]$ make package/shadowsocks-openwrt/libev/install
    ...
    [haohaolee@arch OpenWrt-SDK]$ make package/shadowsocks-openwrt/shadowsocks-libev/install
    ...
    
Finally find your package in dir bin

[dev]: https://dev.openwrt.org
[downloads]: http://downloads.openwrt.org/