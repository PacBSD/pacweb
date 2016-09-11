+++
banner = ""
categories = []
date = "2016-09-07T19:43:57-04:00"
images = []
menu = ""
tags = []
title = "PacBSD Downloads"
url = "/download"

+++

## Release Info

We provide two different images a ISO for burning to a CD/DVD, and a IMG file for
flashing to a USB stick using a utility like `dd`.  Both images are intended for
new installations only; an existing PacBSD system can always be updated with
`pacman -Syu`.

{{< images guide="#" bugs="#" lists="#">}}

## Existing PacBSD Users

If you are an existing PacBSD user, there is no need to download a new image to
update your existing system. You may be looking for an [updated mirrorlist](#)
instead.

## BitTorrent Download (recommended)

If you can spare the bytes, please leave the client open after your download is
finished, so you can seed it back to others. A web-seed capable client is
recommended for fastest download speeds.

*   [ISO torrent file](#)
*   [IMG torrent file](#)

## HTTP Direct Downloads

In addition to the BitTorrent links above, install images can also be downloaded
via HTTP from the mirror sites listed below. Please ensure the download image
matches the checksum from the md5sums.txt or sha1sums.txt file in the same
directory as the image.

### PGP Signature

File validity can be checked with the following [signature file](#).


### Checksums

File integrity checksums for the latest releases can be found below:

#### ISO Installer

{{< checksums iso >}}

#### IMG Installer

{{< checksums img >}}

### Mirrors

{{< mirrorlists >}}

If you want to become an Official PacBSD Mirror please follow the
instructions listed
[here](https://wiki.pacbsd.org/index.php/DeveloperWiki:NewMirrors).
