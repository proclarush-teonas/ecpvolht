# ecpvolht

Eon CheckPoint VPN on Linux How-To

1. extract `pkcs12` package into CA cert, client cert and private key https://stackoverflow.com/a/9516936/2915423 (optionally drop private key passphrase)
1. install shrew vpn client (package called `ike` on Ubuntu/Debian, google the package name for your specific distro OR [build frou source code](https://www.centos.org/forums/viewtopic.php?t=49096))
1. configure as suggested on attached [screenshots](https://github.com/helvete/ecpvolht/tree/master/screenshots), OR import [site config](https://github.com/helvete/ecpvolht/blob/master/shrewsoft_vpn_config/config.vpn) and replace cert files & private key @ credentials tab
1. run key service daemon (via provided [ikedsvc](https://github.com/helvete/ecpvolht/blob/master/src/ikedsvc) init script or manually)
1. launch the GUI (`qikea`), configure the site, create tunnel and enjoy
