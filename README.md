# Version #
v.3.0.2

This is a system to automate the installation of ISPConfig 3 control Panel ( http://www.ispconfig.org/page/home.html ).

Tested on:

- Debian 9 Stretch ([Servisys VPS](https://www.servisys.it/), VmWare Esxi, Amazon AWS, Virtualbox, OVH VPS, Hetzner, Digital Ocean)
- Debian 8 Jessie ([Servisys VPS](https://www.servisys.it/), VmWare Esxi, Amazon AWS, Virtualbox, OVH VPS, Hetzner, Digital Ocean)
- Debian 7 Wheezy ([Servisys VPS](https://www.servisys.it/), VmWare Esxi, Amazon AWS, Virtualbox, OVH VPS, Hetzner, Digital Ocean)
- Ubuntu 14.04 Trusty ([Servisys VPS](https://www.servisys.it/), VmWare Esxi, Amazon AWS, Virtualbox, OVH VPS, Hetzner, Digital Ocean)
- Ubuntu 15.10 Willy ([Servisys VPS](https://www.servisys.it/), VmWare Esxi, Amazon AWS, Virtualbox, OVH VPS, Hetzner, Digital Ocean)
- Ubuntu 16.04 Xenial Xerus ( [Servisys VPS](https://www.servisys.it/), VmWare Esxi, Amazon AWS, Virtualbox, OVH VPS, Hetzner, Digital Ocean)
- Centos 7 ([Servisys VPS](https://www.servisys.it/), Vitualbox)
- ISPConfig 3.*

For now it is tested and developed only on Debian systems.

Maybe it works well also on Ubuntu systems.

### What is this repository for? ###

This repository contains some scripts for the automation

of installation of ISPConfig 3 control panel.

Before start be sure to configure your server following the following guides:

- Debian 9: https://www.howtoforge.com/tutorial/debian-minimal-server/
- Debian 8: https://www.howtoforge.com/tutorial/debian-8-jessie-minimal-server/
- Debian 7: https://www.howtoforge.com/perfect-server-debian-wheezy-apache2-bind-dovecot-ispconfig-3
- Ubuntu 14.10: https://www.howtoforge.com/tutorial/ubuntu-minimal-server-install/
- Ubuntu 15.10: https://www.howtoforge.com/tutorial/ubuntu-minimal-server-install/
- Ubuntu 16.04: https://www.howtoforge.com/tutorial/ubuntu-minimal-server-install/
- Centos 7: http://www.howtoforge.com/centos-7-server

You can Choose during install:
- Apache / Nginx
- Dovecot or Courier
- Quota On/Off
- Jailkit On/Off
- Squirrelmail / Roundcube
- ISPConfig 3 Standard / Expert mode
- ISPConfig 3 Multiserver Setup (* Debian 8 only for now)

### How do I get set up? ###

* Summary of set up

First of all follow the guide 

https://www.howtoforge.com/perfect-server-debian-wheezy-apache2-bind-dovecot-ispconfig-3

to install debian as required for ISPConfig

* Configuration for Debian 7 / 8 / 9 - Ubuntu 14.04 / 15.10 / 16.04

After you got a fresh and perfect Debian installation you had to

```shell
cd /tmp; wget --no-check-certificate -O installer.tgz "https://github.com/servisys/ispconfig_setup/tarball/master"; tar zxvf installer.tgz; cd *ispconfig*; bash install.sh
```
* Centos 7

```shell
cd /tmp; yum install wget unzip net-tools; wget --no-check-certificate -O installer.tgz "https://github.com/servisys/ispconfig_setup/tarball/master"; tar zxvf installer.tgz; cd *ispconfig*; bash install.sh
```

Centos 7 is in a very early stage, we got to test a bit, any help will be appreciated. 
Some feature are missing for now, only implemented Apache and Dovecot, no webmail.

Follow the instruction on the screen
