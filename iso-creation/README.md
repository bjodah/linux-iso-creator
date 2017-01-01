ISO Creation
============

Following the tutorial at https://help.ubuntu.com/community/LiveCDCustomizationFromScratch

Customization
-------------

You may wan to change the following variables in the
[configuration.sh](configuration.sh) file:

- `ARCH` is the architecture of the live cd.
  Example: `amd64`. See [here][chroot].
- `RELEASE` is the release of the live cd.
  If it has the value `xenial`, it uses ubuntu 16.4
  See [here][chroot] for why it is used.
  See [here][ubuntu-releases] for a list of ubuntu releases.
  If you change the release, also change [the sources][h-sources]

Sources
-------

The [sources.list](sources.list) file is generated from
[this form][sources-generator].
Please put the output of the website into the following files:

- [sources.list](sources.list) for the **Sources List**.
- [gpg-keys.sh](gpg-keys.sh) for the **GPG Keys**




[sources-generator]: https://repogen.simplylinux.ch/
[chroot]: https://help.ubuntu.com/community/LiveCDCustomizationFromScratch#Make_the_ChRoot_Environment
[ubuntu-releases]: https://wiki.ubuntu.com/Releases
[h-sources]: #sources