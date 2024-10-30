# Software Management

A package management system is a collection of tools to automate the process of installing, upgrading, configuring, and removing software packages from a computer

**APT-GET**

**apt-get**: is a simple command line interface for downloading and installing packages. The most frequently used commands are update and install.


Red Hat based:

*.RPM
rpm
yum

Debian based:

*.DEB
pkg
apt

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
