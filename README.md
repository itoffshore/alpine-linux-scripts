# alpine-linux-scripts
Alpine Linux Setup Scripts

Boot an [Alpine Linux iso](http://alpinelinux.org/downloads/) &:

    setup-interfaces # <enter> x 3
    ifup eth0
    setup-apkrepos   # choose one near you
    apk add wget ca-certificates
    wget http://it-offshore.co.uk/alpine/setup-disk
    wget http://it-offshore.co.uk/alpine/setup-partitions
    chmod +x set*
    ./setup-partitions
    ./setup-disk -m sys -E # hard disk encrypted installation
