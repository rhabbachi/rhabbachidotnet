+++
date = "2017-01-11T16:07:48+01:00"
title = "Building home server"
tags = []
categories = []
draft = true
+++

### References
- https://wiki.archlinux.org/index.php/Wireless_network_configuration#Manual_wireless_connection_at_boot_using_systemd_and_dhcpcd
- http://unix.stackexchange.com/questions/173781/how-can-i-enable-wpa-supplicant-on-boot
- http://askubuntu.com/questions/503397/how-do-i-install-wpa-supplicant-on-an-offline-server
- https://www.joachim-breitner.de/blog/664-Switching_to_systemd-networkd
- https://wiki.archlinux.org/index.php/Wireless_network_configuration#Wireless_management
- https://wiki.archlinux.org/index.php/WPA_supplicant

# Disk
http://bindfs.org/docs/bindfs.1.html

# Mosh
https://mosh.org/
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-mosh-on-a-vps
https://www.digitalocean.com/community/tutorials/how-to-configure-tmux-on-a-cloud-server
https://blog.filippo.io/my-remote-shell-session-setup/

zplug does not like dotfiles inside it's .zplug directory
Manually install vundle plugin.
'Completor requires vim compiled with python or python3 and has features `job`, `timers` and `lambda`'
vim --version > 8.0

sudo add-apt-repository ppa:jonathonf/vim

first time using the new `apt` command. looks cool.
tmux needed to manually install the tpm plugin https://github.com/tmux-plugins/tpm
git diff-highlight missing
$ sudo add-apt-repository ppa:git-core/ppa

# ssh key
`ssh-copy-id`
`.ssh/config`

# Dyn DNS
Going with nsupdate.info
Found about OVH DynHost
https://docs.ovh.com/fr/fr/web/domains/utilisation-dynhost/
It works with ddclient!
https://p3ter.fr/gestion-du-dyndns-sous-linux-avec-ovh.html
https://wiki.archlinux.org/index.php/Dynamic_DNS
https://www.perhonen.fr/blog/2016/03/dynhost-dyndns-de-chez-ovh-2446

# Docker
install default/vetted repos.
install docker-composer from https://docs.docker.com/compose/install/
all base docker-compose.yml were too complicated for my liking. started off https://gist.github.com/EloB/123cae096cddd9c1712e

# Docker services
## Borg

## Nextcloud
https://docs.docker.com/compose/environment-variables/
https://hub.docker.com/r/wonderfall/nextcloud/~/dockerfile/
https://docs.docker.com/compose/environment-variables/
https://help.nextcloud.com/t/large-dataset-initial-import-rsync-supported/5414/4

## proxy
https://github.com/jwilder/nginx-proxy
https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion
https://github.com/fatk/docker-letsencrypt-nginx-proxy-companion-examples
http://jasonwilder.com/blog/2014/03/25/automated-nginx-reverse-proxy-for-docker/

## PI-Hole
https://pi-hole.net/
https://github.com/pi-hole/pi-hole
https://discourse.pi-hole.net/t/howto-using-pi-hole-as-lan-dns-server/533/2
https://www.reddit.com/r/pihole/comments/4bsb84/use_pihole_to_resolve_local_dns/?st=iz2lb0cy&sh=71166c88
https://hub.docker.com/r/diginc/pi-hole/
https://github.com/diginc/docker-pi-hole
http://superuser.com/questions/367969/how-can-i-direct-a-query-to-specific-dns-server

# Docker systemd integration
https://forums.docker.com/t/how-to-make-a-systemd-unit-for-docker-compose/26199/2
https://github.com/docker/compose/issues/4266
http://stackoverflow.com/questions/41598526/how-does-docker-compose-start-container-on-login-ubuntu-systemd
https://docs.docker.com/engine/admin/host_integration/
https://github.com/andreaskoch/dcsg
