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
