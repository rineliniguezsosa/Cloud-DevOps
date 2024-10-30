# Software Management

A package management system is a collection of tools to automate the process of installing, upgrading, configuring, and removing software packages from a computer

**APT-GET**

**apt-get**: is a simple command line interface for downloading and installing packages. The most frequently used commands are update and install.

- update - Retrieve new lists of packages
- upgrade - Perform an upgrade
- install - Install new packages (pkg is libc6 not libc6.deb)
- remove - Remove packages
- purge - Remove packages and config files
- check - Verify that there are no broken dependencies

**apt-cache**: is a low-level tool used to manipulate APT's binary cache files, and query information from them.

- showpkg - Show some general information for a single package
- search - Search the package list for a regex pattern
- show - Show a readable record for the package
- depends - Show raw dependency information for a package

Red Hat based:

*.RPM
rpm
yum

Debian based:

*.DEB
pkg
apt

**Alternatives**

**alternatives** creates, removes, maintains and displays information about the symbolic links comprising the alternatives of software, that is installed on the system, like several versions of java, python, ruby, nodejs, etc.

- alternatives [options] --install link name path priority [--slave link name path]... [--initscript service]
- alternatives [options] --remove name path
- alternatives [options] --set name path
- alternatives [options] --auto name
- alternatives [options] --display name
- alternatives [options] --config name

**Systemd/init.d**

**init.d**: The init.d directory contains a number of start/stop scripts for various services on your system.

/etc/init.d/command OPTION

Where command is the actual command to run and OPTION can be one of the following:

- start
- stop
- reload
- restart
- force-reload

**Cron**

**cron**: daemon to execute scheduled commands

**EDIT**

To add or update job in crontab, use below command. It will open crontab file in the editor where a job can be added/updated.

```sh
crontab -e
```

By default, it will edit crontab entries of current logged in user. To edit other user crontab use command as below

```sh
crontab -u username -e
```
There are two types of crontab files. The system-wide crontab files and individual user crontab files.