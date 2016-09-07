+++
banner = ""
categories = ["News"]
date = "2013-02-22T00:00:00-04:00"
images = []
menu = ""
tags = ["New ISO"]
title = "ISO Now Available for Testers"

+++

The ISO is now available for testing, which can be found at
[ftp](ftp://ftp.archbsd.net/iso/); Only x86_64 is available at this moment.

[ZFS Install Guide](http://wiki.archbsd.net/index.php/Official_Arch_BSD_ZFS_Install_Guide)

[UFS Install Guide](http://wiki.archbsd.net/index.php/Official_Arch_BSD_Install_Guide)

While everything is still in infancy you should be able to install and get X up and running.

All of the core packages are compiled with clang 3.1 and have been signed, as for extra packages these currently aren't signed yet so must have:

 SigLevel = Never

in

 /usr/local/etc/pacman.conf

This is already set on the iso, however, the pacman package ships the config with this set to require package signing, so must be disabled after install for now.

The follow packages are available for testing X

*   Xorg-server 1.13
*   Mesa 9.0
*   xf86-video-vesa
*   openbox
*   i3

Note the nvidia binary blob drivers have a PKGBUILD at
[github](https://github.com/Amzo/ArchBSD/tree/master/extra/nvidia)

The packages are still very limited at this time, as this release is to get the iso and base packages tested to have any problems fixed.

There is still a lot of work on the website to be done that I yet haven't had time to get around to doing.

However most things are currently working, so if you have any issues or
[bugs](http://bugs.archbsd.net/) to submit please do so, so they can be fixed.

If you wish to request a PKGBUILD ask on the [forum](http://bbs.archbsd.net/),
or feel free to submit your own to the [aur](http://aur.archbsd.net/).

Information on making PKGBUILDS for ArchBSD can be found
[here](http://wiki.archbsd.net/index.php/PKGBUILD)

You can find me on IRC at irc.ircstorm.net #ArchBSD
