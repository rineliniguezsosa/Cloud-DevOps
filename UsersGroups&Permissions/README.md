# Users and Groups

Each user in UNIX has the following parameters:

- User name
- Encrypted password (or 'x' if hash is stored)
- User Identifier (UID)
- Group Identifier (GID)
- Full name or description
- User’s home directory
- User’s shell
- Expiration date
- Each group in UNIX has the following parameters:

Group name
- Encrypted password (or 'x' if hash is stored)
- Group Identifier (GID)

Information about all users you can find in file **/etc/passwd**
Information about these groups you can find in file **/etc/group**

**Operations**

User:

- su
- sudo
- useradd
- userdel
- usermod
- passwd
- finger

Groups:

- groupadd
- groupdel
- groupmod
- groups

**Substitute User**

**su**: switch between users

```sh
su root
```

**Super user do**

**sudo**: run programs with the security privileges of another user.

**Add user**

**useradd**: create user (requires root access)

```sh
useradd –d /home/mydir –s /bin/bash user1
```

**options**

- d: The new user will be created using HOME_DIR as the value for the user's login directory
- s:  The name of the user's login shell