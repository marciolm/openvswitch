Note: patch is already avaiable at http://patchwork.openwrt.org/patch/4343/

So I don't need to use this feed any longer...


Installation in OpenWrt


    $ cd $TOPDIR
    $ echo 'src-git openvswitch git://github.com/alexanderplatz1999/openvswitch.git' >> feeds.conf
    $ ./scripts/feeds update openvswitch
    $ ./scripts/feeds install -a -p openvswitch
    $ make menuconfig
     
    CONFIG_PACKAGE_kmod-crypto-crc32c=y
    CONFIG_PACKAGE_kmod-lib-crc32c=y
    CONFIG_PACKAGE_kmod-openvswitch=m
    CONFIG_PACKAGE_openvswitch-common=m
    CONFIG_PACKAGE_openvswitch-controller=m
    CONFIG_PACKAGE_openvswitch-switch=m

