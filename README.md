Notes
=====

Run on a freshly installed server under root, may not work under an already setup server!

No warranty. For help visit #minstall on Freenode and ask your question (I'm busy with school so response times may be slow...)

Compatibility
=============

**Operating Systems:**

 + Debian 7 (Wheezy) 64 Bit
 + Debian 7 (Wheezy) 32 Bit
 + Ubuntu 12.04 (Precise Pangolin) 32 Bit
 + Ubuntu 12.04 (Precise Pangolin) 64 Bit

**Platforms:**

 + Hardware
 + KVM
 + OpenVZ
 + VirtualBox
 + VMware
 + vServer (Debian Only)
 + Xen HVM
 + Xen PV

Instructions
============

This script contains several modules designed to help you set up your server how you want it. Simply run the below download command then run "bash minstall.sh help" or "bash minstall.sh modules" to see help or modules respectively.

**Download Minstall**

To download Minstall to your home directory (it's recommended that you download and run as root) use the following command:

	wget --no-check-certificate -O minstall.tar.gz http://www.github.com/KnightSwarm/Minstall/archive/2.5.7.tar.gz; tar zxvf minstall.tar.gz; rm minstall.tar.gz; cd Minstall-2.5.7

**Upgrading Packages**

To upgrade your installed packages regularly and retain Minstall system structure it's recommended that you use the following command:

	bash minstall.sh configure-upgrade

**Remove Minstall**

To remove the Minstall script run the following command under the same user you installed Minstall under:

	cd ~; rm -rf minstall

Sample Commands
===============

**Install**

	bash minstall.sh install-extra-repositories
	bash minstall.sh clean-packages
	bash minstall.sh install-ssh
	bash minstall.sh install-extra-packages

**Configure**

	bash minstall.sh configure-general
	bash minstall.sh configure-ssh
	bash minstall.sh configure-upgrade
	bash minstall.sh configure-user

**HTTP**

	bash minstall.sh http-install-exim
	bash minstall.sh http-install-mysql
	bash minstall.sh http-install-nginx
	bash minstall.sh http-install-php
	bash minstall.sh http-install-php-extra
	bash minstall.sh http-configure-mysql
	bash minstall.sh http-configure-nginx

**Manage**

	bash minstall.sh manage-add-user
	bash minstall.sh manage-add-host
	bash minstall.sh manage-manage-user
	bash minstall.sh manage-manage-host
	bash minstall.sh manage-remove-host
