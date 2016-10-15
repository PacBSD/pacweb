+++
draft = false
categories = [
  "News",
]
tags = [
  "Intervention Required",
  "Manual Package Update"
]
menu = ""
banner = ""
images = [
]
date = "2016-10-15T00:00:00-04:00"
title = "Package Signing Key Update"

+++

Due to one of the package signing key expiring manual intervention is required
to update or for new installs.

## For New Installs

For new installs until a new installation image is generated the `SigLevel`
setting in _/etc/pacman.conf_ needs to be set to `Never`.

Change:

    SigLevel = Required DatabaseOptional

To:

    SigLevel = Never

From then the install should be able to run as normal, after install the default
setting of `Required DatabaseOptional` can be keep.

## For Existing Installs

For existing users the old GnuPG keychain needs to be removed as the old key has
issues resetting the trust level.  To upgrade the `pacbsd-keychain` package set
`SigLevel` to be Never and upgrade the package:

    # rm -rf /etc/pacman.d/gnupg
    # pacman -Syy
    # pacman -S pacbsd-keyring
    # pacman-key --init
    # pacman-key --populate pacbsd

After that revert the `SigLevel` option of _/etc/pacman.conf_ back to the
original `Required DatabaseOptional` setting.
