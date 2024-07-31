# UNIX
A repository for UNIX command lines

## Introduction
- Unix is an Operating System that is truly the base of all Operating Systems like Ubuntu, Solaris, POSIX, etc.
- In unix, commands are entered into a shell
  - Locally at the server or remotely, usually over SSh
  - The shell interacts with the Unix kernel.
  - Different shells have different syntax.
- Some commnds require root access - use "sudo" or "su"
- Everything is case sensitive
- Unix has "Man"ual pages
  - Provides help for Unix Commands
  - Examples:
      - man 5 crontab (Configuration file help)
      - man 1 ls (1 means it is a standard user cmd)
      - man 8 ping (8 means it is a system admin cmd)

--------
## Unix Command Overview

### Common Unix Commands:

| Command | Description |
| ------- | ----------- |
| ls      | List directory contents |
| cd      | Change directory |
| pwd     | Print working directory |
| mkdir   | Makes new directory |
| rm      | Removes file or directory |
| cp      | Copy |
| mv      | Move / Rename |
| tar     | Tape archiving |
| chmod   | Set file system permissions |
| whoami  | Show current login name |
| passwd  | Set current user password |
| ssh     | Use secure shell to remotely manage a host |
| logout  | Log current user out |
| grep    | Line filtering |
| awk     | Regular expression filtering |
| cat     | Display text file contents  |
| head    | Display first 10 lines from a text file unless specified |
| tail    | Display last xx lines from a text file |
| vi      | Standard text editor |
| vim     | Standard text editor |
| nano    | Standard text editor |
| df      | Disk free |
| top     | Show top running processes |


### Unix Concept - Piping
- Uses the "|" symbol
- passes the result of the command on the left to the command to the right of the pipe
  - eg. ifconfig | grep inetaddr
- The passed data is text
  - So text parsing, filtering and manipulation could be required.

### Common Unix Shells
- bash /sh
- korn
- c shell
- zsh

> [!TIP]
> View current shell by echo $shell

> [!TIP]
> To change to a C shell while logged in: tcsh

> [!TIP]
> To permanently change to a C shell: chsh

### Common Unix Shell Variables
- $USER
- $SHELL
- $PATH
- $DISPLAY
- $EDITOR

--------

## Advanced GNU & UNIX Commands

| Command | Description |
| ------- | ----------- |
| tac     | Will display the contents of the file in reverse order |
| /       | to search for a something in a file. |
| nl      | line numbering when opening a file |
| wc      | Returns word count in t he format - Lines Words BytesOfData |
| od      | Octal dump |
| pr      | Opens the file in a report format with date and page number |
| join    | Joins the files |


----------

## UNIX File System

| Partition | Mountpoint | File System | Options | Backed up by dump? | FSCK Check Order Upon Boot |
| --------- | ---------- | ----------- | ------- | ------------------ | -------------------------- |
| /da0p1    | / | ufs or zfs or jfs or etc | rw or r or w | 1 or 0 | 1 or 0 |
