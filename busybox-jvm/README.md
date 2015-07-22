# docker-busybox-jvm

Prepare busybox to install a jvm 32 bits in /usr/lib/jvm/jre.

## Supported tags and respective `Dockerfile` links

-	[`latest` (*Dockerfile*)](https://github.com/ofayau/docker-busybox-lib32/blob/master/busybox-jvm/Dockerfile)

## Details

This image :

- is a base for any 32 bits JVM image. It sets $PATH and $JAVA_HOME to `/usr/lib/jvm/jre`.

- is an extension of the [docker-busybox-lib32](../docker-busybox-lib32/) image

## License

- *Busybox* : see [license information](http://www.busybox.net/license.html).

- *Debian libc-i386* : see [licence](http://ftp-master.metadata.debian.org/changelogs//main/g/glibc/glibc_2.19-18_copyright) of [debian package](https://packages.debian.org/jessie/libc6-i386).

