+++
date = "2017-01-05T17:43:51+01:00"
title = "Use an External Thumbdrive when using Company Laptop"
categories = []
tags = []
draft = true
+++

### Backgound Story
### Solution
The moment I realized this need, I went ahead and bought a 32G [SANDISK ULTRA
DUAL](https://www.sandisk.com/home/mobile-device-storage/ultra-dual-usb-drive-3).
This will make it easier for me to use the data for my day to day usage on my
company laptop, as well as occationally be able to access credentials and such
that I don't want to share with for profits services on my Android Phone
(Ironically also provided by $day_job).

### Quick n Dirty: Symlincs

### BindFS to the rescuse
BindFS is kinda link simlinking but on steroids.
This gave me the opportunity to clean-up my fstab file.
###### References
- [permissions - How does one permissibly access files on non-booted system's user's home folder? - Unix & Linux Stack Exchange](http://unix.stackexchange.com/questions/190866/how-does-one-permissibly-access-files-on-non-booted-systems-users-home-folder)
- [filesystems - What is a bind mount? - Unix & Linux Stack Exchange](http://unix.stackexchange.com/a/198591/100187)
- [linux - Permissions on private key in .ssh folder? - Super User](http://superuser.com/a/215506/652566)
- [bindfs](http://bindfs.org/)
- [BINDFS(1) manual page](http://bindfs.org/docs/bindfs.1.html)
- [linux - What are the correct permissions for the .gnupg enclosing folder? gpg: WARNING: unsafe enclosing directory permissions on configuration file - Super User](http://superuser.com/a/954536/652566)
