# Alpine Linux Setup Scripts

To install to **`gpt` disks** you will need to choose a **`(b)oot` disk layout** in `setup-partitions` for the `boot` drive to be confgured correctly.

## Boot an [Alpine Linux iso](http://alpinelinux.org/downloads/) &:

```sh
setup-interfaces # <enter> x 3
ifup eth0
setup-apkrepos   # choose one near you
apk add wget ca-certificates
wget http://it-offshore.co.uk/alpine/setup-disk       #redirects to raw github script
wget http://it-offshore.co.uk/alpine/setup-partitions #redirects to raw github script
chmod +x set*
./setup-partitions
./setup-disk -m sys -E # hard disk encrypted installation
```

[![asciicast](https://asciinema.org/a/18354.png)](https://asciinema.org/a/18354)
[![asciicast](https://asciinema.org/a/18130.png)](https://asciinema.org/a/18130)
[![asciicast](https://asciinema.org/a/22619.png)](https://asciinema.org/a/22619)
