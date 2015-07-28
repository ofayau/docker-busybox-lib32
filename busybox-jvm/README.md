# docker-busybox-jvm

Prepare busybox to install a 32 bits JVM.

## Supported tags and respective `Dockerfile` links

-	[`latest` (*Dockerfile*)](https://github.com/ofayau/docker-busybox-lib32/blob/master/busybox-jvm/Dockerfile)

## Details

This image :

- is a base for any 32 bits JVM image. It sets `$PATH` and `$JAVA_HOME` to `/usr/lib/jvm/jre`.

- is an extension of the [docker-busybox-lib32](https://github.com/ofayau/docker-busybox-lib32/tree/master/busybox-libc32) image

## Comparison

Compared to some 64 bits JVM images :

```sh
REPOSITORY                  TAG          IMAGE ID        CREATED         VIRTUAL SIZE
frolvlad/alpine-oraclejdk8  latest       8e87306ea37d    7 weeks ago     170.4 MB
jeanblanchard/busybox-java  8            f9b532dbdd9f    3 months ago    162 MB
java                        8-jre        b0f21df5333b    5 months ago    478.7 MB
```

This allow very tiny JVM images :

```sh
REPOSITORY                  TAG          IMAGE ID        CREATED         VIRTUAL SIZE
ofayau/j2me                 latest       f56c31b1cc20    26 hours ago    21.73 MB
ofayau/ejre                 8-compact1   824a6f1a0ade    4 minutes ago   39.31 MB
ofayau/ejre                 8-compact2   9da39771057a    4 minutes ago   44.85 MB
ofayau/ejre                 8-compact3   a9fbe6b90034    4 minutes ago   48.79 MB
ofayau/ejre                 8-jre        d5ed29a4bf44    4 minutes ago   80.66 MB
ofayau/openjdk              8-compact1   f258bd30ec46    5 days ago      47.08 MB
ofayau/openjdk              8-compact2   dc125eeac09b    5 days ago      59.82 MB
ofayau/openjdk              8-compact3   b10fc16f53ea    5 days ago      66.38 MB
ofayau/openjdk              8-jre        fded935a77ed    5 days ago      115.1 MB
```

Discover these images :

- [`ofayau/openjdk` (*OpenJDK*)](https://registry.hub.docker.com/u/ofayau/openjdk/)
- [`ofayau/ejre` (*Oracle Java SE Embedded*)](https://registry.hub.docker.com/u/ofayau/ejre/)
- [`ofayau/j2me` (*Oracle Java ME*)](https://registry.hub.docker.com/u/ofayau/j2me/)

## License

- *Busybox* : see [license information](http://www.busybox.net/license.html).

- *Debian libc-i386* : see [licence](http://ftp-master.metadata.debian.org/changelogs/main/g/glibc/glibc_2.19-18_copyright) of [debian package](https://packages.debian.org/jessie/libc6-i386).

