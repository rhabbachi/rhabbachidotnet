+++
title = "Rpi Nas Docker Machine"
date = 2017-09-25T10:36:14+01:00
tags = []
categories = ["post"]
draft = true
+++

|

The main objectives for this raspberrypi system setup are:

### Backups!
Make this huge 5 hard drives enclosure that I had since 2 years now and failed
to make it a consistant part of my backup strategy.

### Network monitoring and filtering (PI-Hole)
I always wanted to have more controle over the home network and my internet
ADSL connection. And I really liked the idea of https://github.com/pi-hole

### Active system
I always thought about having a malleable always on system available on the
network. Having a VPS hosted remotly was kinda difficult mainly to me feeling .
Maybe a future DIY home automation setup?

## PI-Hole
- https://github.com/pi-hole
- https://hub.docker.com/r/diginc/pi-hole/

SMB vs NFS authentication: https://serverfault.com/questions/597254/smb-vs-nfs-authentication
Resinos: https://resinos.io/#downloads-raspberrypi
"docker arm exec format error"
5 things about Docker on Raspberry Pi: https://blog.alexellis.io/5-things-docker-rpi/
theopenbit/rpi-nfs-server: https://hub.docker.com/r/theopenbit/rpi-nfs-server/
https://github.com/cpuguy83/docker-nfs-server
https://github.com/jcbiellikltd/docker-nfs4
https://github.com/f-u-z-z-l-e/docker-nfs-server
https://github.com/sjiveson/nfs-server-alpine
https://blog.alexellis.io/hardened-raspberry-pi-nas/
https://blog.alexellis.io/mutli-stage-docker-builds/
https://docs.docker.com/engine/userguide/eng-image/multistage-build/#name-your-build-stages
https://github.com/docker-library/official-images#multiple-architectures
https://github.com/kelseyhightower/confd/

## Borg
- b3vis/borg-server: https://hub.docker.com/r/b3vis/borg-server/
- b3vis/borg-server: https://github.com/b3vis/borg-server

## Gogs server
- git-server-docker: https://github.com/shoonoise/git-server-docker
- Gogs: https://gogs.io
- Gogs Configuration: https://gogs.io/docs/installation/configuration_and_run
- gogs/gogs-rpi: https://hub.docker.com/r/gogs/gogs-rpi/
- gogits/gogs: https://github.com/gogits/gogs/pull/4431
- Run your own GitHub-like service with the help of Docker: https://blog.hypriot.com/post/run-your-own-github-like-service-with-docker/
- hypriot/rpi-gogs-alpine: https://hub.docker.com/r/hypriot/rpi-gogs-alpine/
- hypriot/rpi-gogs-raspbian: https://github.com/hypriot/rpi-gogs-raspbian

## Laptop integration
- networkmanager dispatcher: adding NFS-shares: https://bbs.archlinux.org/viewtopic.php?id=118335

## Future?
- https://hub.docker.com/r/hypriot/rpi-gpio/
