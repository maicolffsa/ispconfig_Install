

En este script se corrige el problema de conexion refusa al servidor de www.ispconfig.org 


# Version #
<b>v.3.0.6</b>

Debian 10 fix for Debian 10

<b>v.3.0.5</b>

Debian 10 changes file path, for root use :

	su -
	
Added support for Debian 10 Buster and php7.3
	service changed to systemctl for all service functions (start,stop,restart etc)
	few other minor changes to accommodate Debian 10

<b>v.3.0.4</b>

This is a system to automate the installation of ISPConfig 3 control Panel ( http://www.ispconfig.org/page/home.html ).



### How do I get set up? ###

Follow one of the above guides to install a fresh copy of a supported Linux distribution.

Run the following command as root user:

* Debian 7, 8, 9 and 10 and Ubuntu 14.04, 15.10, 16.04, 16.10 and 18.04

```shell
cd /tmp; wget -O installer.tgz "https://github.com/maicolffsa/ispconfig_install/tarball/master"; tar zxvf installer.tgz; cd *ispconfig*; bash install.sh
```

* Armbian 20.04

```shell
cd /tmp; wget -O installer.tgz "https://github.com/maicolffsa/ispconfig_install/tarball/master"; tar zxvf installer.tgz; cd *ispconfig*; bash installArmbian.sh
```

* Raspbian 20.04

```shell
cd /tmp; wget -O installer.tgz "https://github.com/maicolffsa/ispconfig_install/tarball/master"; tar zxvf installer.tgz; cd *ispconfig*; bash installRaspbian.sh
```

* CentOS 7

```shell
cd /tmp; sudo yum install wget unzip net-tools; wget -O installer.tgz "https://github.com/maicolffsa/ispconfig_install/tarball/master"; tar zxvf installer.tgz; cd *ispconfig*; sudo install.sh
```

CentOS 7 is in a very early stage, we got to test a bit, any help will be appreciated. 
Some features are missing for now, only implemented Apache and Dovecot, no webmail.

If `wget` fails, try adding the `--no-check-certificate` parameter.

Follow the instructions on the screen

### Who had contributed to this work? ###

* The scripts and instructions have been produced by Matteo Temporini ( <temporini.matteo@gmail.com> )
* Special thanks to Travis CI for adding support to Raspberry and a big number of Bugs( https://github.com/tdulcet )
* Special thanks to Torsten Widmann for contribution to the code
* Special thanks to Michiel Kamphuis ( http://www.ensync.it/ ) for contribution to Multiserver Setup integration
* Special thanks to Bartłomiej Gajda ( http://webard.me/ ) for the bug fixes to multiserver setup and beta installation
* The code is based on the "Automatic Debian System Installation for ISPConfig 3" of Author: Mark Stunnenberg <mark@e-rave.nl>
* Howtoforge community https://www.howtoforge.com/community/
