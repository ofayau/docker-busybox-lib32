# docker-busybox-lib32

Busybox with 32 bits (and 64 bits) libs.

## Supported tags and respective `Dockerfile` links

-	[`latest` (*Dockerfile*)](https://github.com/ofayau/docker-busybox-lib32/blob/master/busybox-libc32/Dockerfile)

## Details

- Docker is exclusively 64 bits.

- For compatiblity reason, 64 bits architecture are able to run 32 bits program.

- Some program (by example java) have 32 bits edition which are smaller than 64 bits.

This docker image add libc 64 bits (in /lib64) and 32 bits libc (in /lib32).

Linux OS will choose what the program need.

## License

- *Busybox* : see [license information](http://www.busybox.net/license.html).

- *Debian libc-i386* : see [licence](http://ftp-master.metadata.debian.org/changelogs//main/g/glibc/glibc_2.19-18_copyright) of [debian package](https://packages.debian.org/jessie/libc6-i386).

