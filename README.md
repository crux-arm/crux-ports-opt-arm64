# crux-ports-opt-arm64

CRUX-ARM aarch64 ports overlay for CRUX opt collection

To use these ports, download the `opt-arm64.httpup` file to `/etc/ports`:
```
$ sudo wget -P /etc/ports https://raw.githubusercontent.com/crux-arm/crux-ports-opt-arm64/3.6/opt-arm64.httpup
$ sudo ports -u opt-arm64
```

You may want to list it first in `/etc/prt-get.conf` to take advantage of ports overlay:
```
###
### prt-get conf
###

# note: the order matters: the package found first is used
prtdir /usr/ports/core-arm64
prtdir /usr/ports/opt-arm64
prtdir /usr/ports/xorg-arm64
prtdir /usr/ports/core
prtdir /usr/ports/opt
prtdir /usr/ports/xorg
```

