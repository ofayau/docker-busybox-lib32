FROM progrium/busybox

MAINTAINER Olivier Fayau <olivier.fayau@gmail.com>

#
# Download & unpack "libc32 for amd64" debian package.
# see https://packages.debian.org/jessie/libc6-i386
#
RUN LIBC32_DEB=libc6-i386_2.19-18_amd64.deb \
  && wget "http://ftp.fr.debian.org/debian/pool/main/g/glibc/$LIBC32_DEB" \
  && echo "5668a0ec3c75dfec4881f7f18b90ad6f  $LIBC32_DEB" | md5sum -c - \
  && ar p $LIBC32_DEB data.tar.xz | unxz | tar -x \
  && rm -rf $LIBC32_DEB /usr/share/doc/libc6-i386 /usr/lib32/gconv /usr/share/lintian

