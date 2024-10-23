# Linux shell basics

**shell types**

- sh
- bash
- csh
- tcsh
- ksh 

**To switch from one shell to another, just enter the name of the new shell in the active terminal.**

**Shell programming**

**environment variables**: In Linux and Unix based systems environment variables are a set of dynamic
 named values, stored within the system that are used by applications and shell scripts launched in 
 shells or subshells. In simple words, an environment variable is a variable with a name and an associated value

 Environment variables allow you to customize how the system works and the behavior of the applications on the
  system or use values of environment variables inside of your shell scripts. For example, the environment variable
   can store information about the default text editor or browser, the path to executable files, or the system locale
    and keyboard layout settings.

```sh
KEY=value
ANOTHER_KEY="Some other value"
KEY_MULTI=value1:value2
```

Variables can be classified into two main categories, **environment variables**, and **shell variables.**

Environment variables are variables that are available system-wide and are inherited by all spawned child processes and shells.

**Shell variables** are variables that apply only to the current shell instance. Each shell such as zsh and bash, 
has its own set of internal shell variables.

