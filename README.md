Supervisor
==========

Supervisor install script

* Installs all dependencies using apt or yum
* Creates init script which is also distro-independent
* Runs update-rc or chkconfig
* Creates config of your choice (default, predefined, open up editor)

Note: Always change the configuration, even the predefined one. If you use the web interface, remember to setup a password and check the port number.

Some program configurations are also included.

Tested on:
* CentOS 5.8/6.4
* Debian 6.0/7.0
* Fedora 17
* Ubuntu 10.04/12.04/12.10/13.04

Default temp dir is ````/tmp/supervisor````, this can be changed in install script.

By default, the installer logs into ````$TMP/install.log```` and ````$TMP/error.log````. Check these for further info about the installation process.

## Dependencies
* Package manager (apt or yum)
* HTTP Client (curl, wget or fetch)
* TAR executable
* Python
* Bash Dialog

Dependencies will be installed during the progress, but installing them on your own is advised.

## Installation

### Online installation

Clone this repository and run ````install.sh````

OR

Just download ````install.sh```` and run it.

### Offline installation

Clone this repository and download the following files manually into the install script path:

[Setuptools 1.0](https://pypi.python.org/packages/source/s/setuptools/setuptools-1.0.tar.gz)

[Supervisor 3.0](https://pypi.python.org/packages/source/s/supervisor/supervisor-3.0.tar.gz)

Run ````install.sh````

This way you can install Supervisor on any machine even without internet connection. Make sure that every dependency is installed.