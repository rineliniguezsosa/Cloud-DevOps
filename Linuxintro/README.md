# Linux introduction

## Concepts

**kernel**: The kernel is a computer program that is the core of a computer's operating system,it is one of the first programs loaded on start-up (after the bootloader)

**Linux distribution**:A Linux distribution is a member of the family of Unix-like software distributions built on top of the Linux kernel

**Shell**: A shell is a program that provides an interface between a user and an operating system (OS) kernel.

**file system** 

**Inode**: The inode (index node) is a data structure in a Unix-style file system that describes a file-system object such as a file or a directory. Each inode stores the attributes and disk block location(s) of the object's data. File-system object attributes may include metadata (times of last change, access, modification), as well as owner and permission data.

**Hard link**
- created with the ln command (and no options) or the link function
- changes made in any reflect in all
- a file is accessible as long as a hard link to it remains

**Soft link**
- a symbolic link (or symlink or soft link) is a pointer to a file name
- if the original file is moved, the link becomes invalid
- usually made to directories to create shortcuts
- created with the -s option to ln or the symlink function

**Logical Volume Manager - LVM**: is a software capability that allows users
administrators combine individual disks and disk partitions and treat them
as if they were a single unit.

**Advantages**
- Use any number of disks as one big disk
- Have logical volumes stretched over several disks.
- Snapshots allow you to backup a frozen copy of the file system, while keeping service downtime to a minimum.
- Resize/create/delete logical and physical volumes online. File systems on them still need to be resized, but some support online resizing

**Disadvantages**
- Additional steps in setting up the system, more complicated.


**Disk Quotas**: Disk space can be restricted by implementing disk quotas which alert a system administrator before a user consumes too much disk space or a partition becomes full