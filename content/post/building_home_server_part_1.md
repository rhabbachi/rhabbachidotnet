+++
date = "2017-01-11T16:07:48+01:00"
title = "Building home server (Part 1: Hardware and initial setup)"
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
https://mosh.org/
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-mosh-on-a-vps
https://www.digitalocean.com/community/tutorials/how-to-configure-tmux-on-a-cloud-server
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
