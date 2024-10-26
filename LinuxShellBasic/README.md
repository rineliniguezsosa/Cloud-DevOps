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

Below are some of the most common environment variables:

- USER - The current logged in user.
- HOME - The home directory of the current user.
- EDITOR - The default file editor to be used. This is the editor that will be used when you type edit in your terminal.
- SHELL - The path of the current user’s shell, such as bash or zsh.
- LOGNAME - The name of the current user.
- PATH - A list of directories to be searched when executing commands.
- Note: When you run a command the system will search those directories in this order and use the first found executable.
- LANG - The current locales settings.
- TERM - The current terminal emulation.
- MAIL - Location of where the current user’s mail is stored.

**When not to use shell scripts**

- Resource-intensive tasks, especially where speed is a factor (sorting, hashing, recursion)
- Complex applications, where structured programming is a necessity (type-checking of variables, function prototypes, etc.)
- Mission-critical applications upon which you are betting the future of the company
- Situations where security is important, where you need to guarantee the integrity of your system and protect against intrusion, cracking, and vandalism
- Need native support for multi-dimensional arrays
- Need data structures, such as linked lists or trees
- Need to generate / manipulate graphics or GUIs
- Need to use libraries or interface with legacy code
- Proprietary, closed-source applications (Shell scripts put the source code right out in the open for all the world to see.)

**Filesystem files search**

**find**: look for files and directories with given criterias

- **name**: buscar archivos o directorios que coincidan con un nombre específico o patrón

**locate** file in filesystem

-  locate passwd

**grep**: print lines matching a pattern

- **grep**: grep -r "fun" ~

**XARGS**

**xargs** - reads arguments from the standard input, separated by blank spaces or newlines

- i:  This  option  is a synonym for -Ireplace-str if replace-str is specified
- cat names.txt | xargs -i touch {}

**Working with Archives**

**ZIP/UNZIP**
- zip -rp <file>.zip /path/to/ #compress folder into .zip
- unzip <file>.zip #extract files in current location from .zip

**TAR**

- c: create a new file tar
- v: muestra los archivos que están siendo procesados (modo verbose)
- f: Especifica el nombre del archivo tar.
- x: Extrae los archivos de un archivo tar.
- t:  Lista el contenido de un archivo tar.
- z: Comprime o descomprime el archivo tar usando gzip.

**GZIP**
gzip, gunzip, zcat - compress or expand files

- gzip -c file1 > foo.gz #compresses file1 into foo.gz.
- gzip -c file2 >> foo.gz #adds file2 into foo.gz.